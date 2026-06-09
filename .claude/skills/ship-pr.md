---
name: ship-pr
description: Commit current changes on a feature branch, push to origin, and open a pull request. Verifies the active gh account matches the repo before pushing. Use when the user wants to ship/commit/push their work, open a PR, or says "commit and push". Never pushes directly to main.
---

Ship the current changes by committing on a feature branch and opening a PR. This skill enforces the user's standard workflow (feature branch → PR → review → merge) and avoids two common pitfalls on this machine:

1. The user has multiple `gh` accounts in keyring (`jarlemeland`, `jarlemaland`). If the wrong one is active, pushes either fail with `403 Permission denied` or get silently parked on `refs/for/<branch>` (a Gerrit-style review ref) by `.storecode` / Rampart safety infrastructure, leaving `main` unchanged on origin and no PR created.
2. Pushing direct to `main` triggers Rampart's "Risky GitHub operation blocked" guard. Always use a feature branch.

## Steps

### 1. Verify the active gh account matches the repo

```bash
gh auth status
git remote -v
```

Extract the repo owner from `origin` (e.g., `github.com/<owner>/<repo>.git`). If the active `gh` account is not `<owner>` (or a known collaborator) and a matching account exists in the keyring, switch:

```bash
gh auth switch --user <owner>
gh auth setup-git   # re-sync git credential helper to the new active account
```

If no matching account is logged in, ask the user to run `gh auth login` manually rather than guessing.

Also sanity-check `git config user.email` matches the GitHub identity if relevant.

### 2. Pre-commit checks (in parallel)

```bash
git status
git diff --stat HEAD
git log --oneline -8     # match commit message style
```

Make sure you're not accidentally including:
- `.storecode/` — local safety infrastructure, never commit
- Secret files (`.env`, credentials)
- Build artifacts (`public/`, `node_modules/`)

### 3. If commits are already on `main` locally, move them to a feature branch first

If `git log origin/main..HEAD` shows commits that should have gone on a branch, fix this BEFORE pushing:

```bash
git checkout -b feat/<descriptive-slug>
# now main can be aligned with origin/main, but git branch -f / git reset --hard
# may be blocked by a safety hook — if so, leave local main as-is and tell the user
# they can sync it after merge with `git checkout main && git fetch && git reset --hard origin/main`
```

### 4. Otherwise commit on a new feature branch

```bash
git checkout -b feat/<descriptive-slug>
git add <explicit paths>           # never `git add -A` — it grabs .storecode/, .env, etc.
git commit -F /tmp/commit-msg.txt  # use a heredoc-written file to avoid shell quoting issues
```

The branch name should be kebab-case and descriptive: `feat/events-styret-ux-fixes`, `fix/nav-aria-current`, `docs/admin-guide`.

### 5. Push the branch

```bash
git push -u origin feat/<slug>
```

If the push returns `refs/for/<branch>` instead of `refs/heads/<branch>`, the wrong gh account was active — see step 1.

If the push returns `403 Permission denied to <other-account>`, run `gh auth setup-git` to re-sync credentials then retry once.

### 6. Open the PR

```bash
gh pr create --base main --head feat/<slug> \
  --title "<short imperative title under 70 chars>" \
  --body "$(cat <<'EOF'
## Summary
- <1-3 bullets describing the change>

## Test plan
- [ ] <how to verify in dev / staging>
- [ ] <build passes / tests pass>
- [ ] <key user flow walks through cleanly>

🤖 Generated with [Claude Code](https://claude.com/claude-code)
EOF
)"
```

Return the PR URL to the user.

## Cleanup if a previous push went to `refs/for/main`

If `git ls-remote origin` shows a stray `refs/for/main` ref from a prior bad push:

```bash
git push origin --delete refs/for/main
```

This is safe — the ref was never a real branch, only a review-queue parking spot.

## What to NEVER do

- Never `git push origin main` directly. Always feature branch + PR.
- Never `git reset --hard` or `git push --force` on `main` to "clean it up" without the user's explicit go-ahead. Local main being temporarily ahead of origin is harmless when the commit also lives on a pushed feature branch.
- Never commit `.storecode/` — it's safety infrastructure with its own gitignore.
- Never `git add -A` or `git add .` blindly — stage explicit paths.
- Never skip hooks with `--no-verify` unless the user asks for it.
