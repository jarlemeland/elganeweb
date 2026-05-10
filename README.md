# Elgane Motorsykkelklubb — Nettside

Nettside for Elgane Motorsykkelklubb, bygget med [Hugo](https://gohugo.io/) og [Decap CMS](https://decapcms.org/). Hostes gratis på [Netlify](https://www.netlify.com/).

## Kom i gang

### Forutsetninger

- [Hugo](https://gohugo.io/installation/) (extended edition, v0.161+)
- [Git](https://git-scm.com/)

### Lokal utvikling

```bash
# Klon repoet
git clone https://github.com/[bruker]/elganeweb.git
cd elganeweb

# Start lokal utviklingsserver
hugo server

# Åpne nettleseren på http://localhost:1313
```

### Bygg for produksjon

```bash
hugo --minify
```

Output havner i `public/`-mappen.

## Prosjektstruktur

```
elganeweb/
├── hugo.toml                  # Hugo-konfigurasjon (menyer, params, etc.)
├── netlify.toml               # Netlify deploy-konfigurasjon
├── content/                   # Alt innhold (Markdown)
│   ├── _index.md             # Forside
│   ├── om-klubben.md         # Om klubben
│   ├── kontakt.md            # Kontaktside
│   ├── treningsplan.md       # Treningsplan-side
│   ├── bane-og-kart.md       # Bane og kart
│   ├── personvern.md         # Personvernerklæring
│   ├── grener/               # Grenersider
│   │   ├── atv-sidevogn.md
│   │   ├── mx.md
│   │   └── speedway.md
│   └── nyheter/              # Nyhetsposter
│       ├── _index.md
│       └── *.md
├── data/
│   └── treninger.yaml        # Treningsplan-data (sikringsledere)
├── layouts/                   # Hugo-templates
│   ├── _default/             # Standard-templates
│   ├── partials/             # Gjenbrukbare deler
│   ├── shortcodes/           # Shortcodes for innhold
│   ├── nyheter/              # Nyhetsspesifikke templates
│   ├── grener/               # Grene-spesifikke templates
│   └── kontakt/              # Kontaktside-template
├── assets/css/main.css        # Alle stiler
├── static/admin/              # Decap CMS (innholdsredigering)
├── i18n/nb.yaml               # Norske oversettelser
├── docs/                      # Dokumentasjon (ikke del av nettsiden)
└── design/                    # Designressurser (ikke del av nettsiden)
```

## Innholdsredigering

### For teknisk admin

Rediger Markdown-filer direkte i `content/`-mappen og push til Git.

**Legge til en nyhetspost:**
```bash
hugo new nyheter/min-nye-post.md
```

### For innholdsprodusenter (ikke-tekniske)

Gå til `https://elgane.no/admin/` og logg inn med e-post/passord.

CMS-et lar deg:
- Skrive og redigere nyhetsposter
- Oppdatere sideinnhold
- **Administrere treningsplanen** — legg til/endre treningsdager med sikringsleder
- Laste opp bilder

Endringer publiseres automatisk på ~30 sekunder.

## Treningsplan

Treningsplanen lagres i `data/treninger.yaml`. Hvert oppføring har:

| Felt | Beskrivelse |
|------|-------------|
| `dato` | Dato (YYYY-MM-DD) |
| `tid_start` | Starttid (HH:MM) |
| `tid_slutt` | Sluttid (HH:MM) |
| `gren` | ATV & Sidevogn, MX, eller Speedway |
| `sikringsleder` | Navn på sikringsleder |
| `status` | bekreftet, avlyst, utsatt, trenger_sikringsleder |
| `merknad` | Valgfri merknad |

Treningsplanen kan redigeres via CMS-et eller direkte i YAML-filen.

## Deployment

Nettsiden deployes automatisk via Netlify når du pusher til `main`-branchen.

**Første oppsett:**
1. Koble repoet til [Netlify](https://app.netlify.com/)
2. Netlify bygger automatisk med `hugo --minify`
3. Aktiver **Netlify Identity** (Site Settings → Identity)
4. Aktiver **Git Gateway** (Identity → Services → Git Gateway)
5. Inviter CMS-brukere via e-post (opptil 5 gratis)

## Teknologi

| Komponent | Teknologi |
|-----------|-----------|
| Rammeverk | Hugo (statisk nettstedgenerator) |
| CMS | Decap CMS (nettleserbasert editor) |
| Hosting | Netlify (gratis tier) |
| CSS | Ren CSS med custom properties |
| Kontaktskjema | Netlify Forms |
| Autentisering | Netlify Identity |

## Kostnader

- **Domene (elgane.no):** ~150–200 NOK/år
- **Hosting:** Gratis (Netlify)
- **CMS:** Gratis (Decap CMS)
- **Totalt:** ~150–200 NOK/år

## Lisens

Vedlikeholdt for Elgane Motorsykkelklubb.
