# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains documentation and resources for the **Elgane Motorsykkelklubb website project**.

Elgane Motorsykkelklubb is a Norwegian motorsport club with three disciplines:
- ATV & Sidecar
- MX (Motocross)
- Speedway

The club is building a new WordPress-based website to replace their current IdrettenOnline platform.

## Technology Stack

**Platform**: WordPress 6.x (self-hosted)
- **CMS**: WordPress (latest stable version)
- **Theme**: Astra (free version)
- **Hosting**: Norwegian budget hosting (One.com, Loopia, or Webhotell.no)
- **Domain**: elgane.no
- **Language**: Norwegian (Norsk Bokmål)

**Essential Plugins**:
- Yoast SEO (search optimization)
- UpdraftPlus (backups)
- Wordfence Security or Solid Security (security)
- Contact Form 7 or WPForms Lite (contact forms)

**Future Plugins** (Phase 2):
- Custom Facebook Feed (Facebook integration)
- The Events Calendar (security leader scheduling)

## Repository Purpose

This is a **documentation repository**, not a code repository. It contains:
- Setup guides and documentation
- Design resources (colors, logos)
- Content templates for initial pages
- Admin user guides
- Hosting provider comparisons

**This repository does NOT contain**:
- WordPress code
- Theme files
- Plugin code
- Database backups

The actual WordPress installation will be hosted on the chosen hosting provider.

## Repository Structure

```
/
├── README.md                          # Project overview and quick start
├── CLAUDE.md                          # This file - development guidance
├── docs/
│   ├── setup-guide.md                # Complete WordPress setup instructions
│   ├── admin-guide.md                # User guide for content managers (Norwegian)
│   ├── hosting-comparison.md         # Norwegian hosting provider comparison
│   └── theme-customization.md        # Astra theme customization guide
├── design/
│   ├── logo/                         # Club logo files (to be added)
│   ├── colors.md                     # Official color scheme documentation
│   └── mockups/                      # Design mockups (optional, to be added)
└── content/
    ├── pages/                        # Content templates for WordPress pages
    │   ├── om-klubben.md            # "About the club" page content
    │   ├── atv-sidecar.md           # ATV & Sidecar branch page
    │   ├── kontakt.md               # Contact page content
    │   └── [other pages]            # Additional page templates
    └── initial-posts.md              # Sample news posts for launch
```

## Working with This Repository

### Adding or Updating Documentation

1. **Documentation is in Markdown**: All docs use Markdown (.md) format
2. **Norwegian content**: Page content and admin guide are in Norwegian (Bokmål)
3. **Technical docs**: Setup guides and technical documentation are in English
4. **Keep it practical**: Focus on actionable, step-by-step guidance

### Design Resources

**Brand Colors**:
- Primary (Elgane Green): `#3fb970`
- Dark background: `#1a1a1a`
- See `design/colors.md` for complete palette

**Logo**:
- Store logo files in `design/logo/`
- Recommended formats: PNG (transparent), SVG, JPG
- Include multiple sizes for different uses

### Content Templates

**Page content** in `content/pages/`:
- Written in Markdown for easy reading
- Contains full page content structure
- Includes notes for WordPress implementation
- Ready to be copied into WordPress

**News posts** in `content/initial-posts.md`:
- Sample posts to launch the site
- Template for future post writing
- Guidelines for categories and formatting

## WordPress Development Guidelines

When working with WordPress for this project:

### Theme Customization (Astra)

**Use the Customizer**:
- Access via: Appearance → Customize
- Most design changes should be made via Customizer
- Click "Publish" to save changes

**Key Areas to Configure**:
1. **Global → Colors**: Set brand colors (#3fb970 primary)
2. **Global → Typography**: Configure fonts (Montserrat/Open Sans recommended)
3. **Header Builder**: Logo, navigation, mobile menu
4. **Footer Builder**: Footer content and layout
5. **Blog/Archive**: Post layout and structure

**Custom CSS**:
- Add via: Customizer → Additional CSS
- Keep custom CSS minimal
- Document any custom CSS added
- See `docs/theme-customization.md` for examples

### Plugin Usage

**Install only necessary plugins**:
- Start with essential plugins only
- Each plugin adds overhead and potential security issues
- Review plugin ratings and update frequency before installing

**Essential plugins** (install immediately):
- Yoast SEO
- UpdraftPlus
- Wordfence or Solid Security
- Contact Form 7

**Future plugins** (Phase 2):
- Custom Facebook Feed (when ready to integrate Facebook)
- The Events Calendar (when calendar feature is needed)

**Avoid**:
- Page builders (Elementor, etc.) unless absolutely necessary
- Plugins that duplicate built-in WordPress features
- Poorly maintained or low-rated plugins

### Content Organization

**Pages vs Posts**:
- **Pages**: Static content (About, Contact, Branch pages)
- **Posts**: News and updates, sorted by date

**Categories for Posts**:
- Nyheter (general news)
- ATV & Sidecar
- MX
- Speedway
- Arrangementer (events)

**Menus**:
- Primary Menu: Main navigation in header
- Footer Menu: Secondary links in footer

### Image Handling

**Image Requirements**:
- Format: JPG for photos, PNG for logos/graphics
- Size: Compress to under 2-5 MB
- Dimensions: Max 1920px width for full-width images
- Always add alt text (accessibility)

**Use Smush plugin** for automatic compression

**Featured Images**:
- Set for all posts
- Recommended ratio: 16:9 or 4:3
- Minimum size: 1200x675px

### Security Best Practices

1. **Keep everything updated**:
   - WordPress core
   - All plugins
   - Theme

2. **Strong passwords**:
   - Minimum 12 characters
   - Mix of letters, numbers, symbols
   - Never use "admin" as username

3. **Backups**:
   - UpdraftPlus configured for weekly backups
   - Store backups off-site (Google Drive, Dropbox)
   - Test restore process

4. **User management**:
   - Give users minimum necessary permissions
   - Administrator: Only for technical admins
   - Editor: For content managers
   - Remove unused accounts

5. **Wordfence/Security plugin**:
   - Enable login security
   - Configure email alerts
   - Run regular scans

### Performance Optimization

**Keep the site fast**:
1. **Image optimization**: Smush plugin
2. **Caching**: Use hosting provider's caching or WP Super Cache
3. **Minimize plugins**: Only essential plugins
4. **Optimize database**: Regular cleanup (WP-Optimize plugin)
5. **CDN**: Consider Cloudflare (free) if needed

**Performance targets**:
- Page load: < 3 seconds
- Google PageSpeed: 70+ mobile, 80+ desktop
- Lighthouse score: 80+ (all metrics)

### Accessibility

**WCAG 2.1 Level AA compliance**:
- Proper heading structure (H1 → H2 → H3)
- Alt text for all images
- Color contrast ratios (4.5:1 minimum for text)
- Keyboard navigation support
- Skip to content link

**Test with**:
- Screen reader (NVDA, JAWS, or VoiceOver)
- Keyboard-only navigation
- WAVE browser extension
- Lighthouse accessibility audit

### Multilingual Support

**Currently**: Norwegian (Norsk Bokmål) only
- WordPress language: Norwegian
- All content in Norwegian
- Admin interface in Norwegian

**Future**: If English version needed, use Polylang or WPML plugin

### Mobile Responsiveness

**Test on**:
- iPhone (Safari)
- Android phone (Chrome)
- iPad/tablet
- Various desktop sizes

**Use Chrome DevTools**:
- Responsive design mode
- Test different viewports
- Check touch targets (minimum 44x44px)

### SEO Guidelines

**On-Page SEO** (via Yoast):
- Meta titles (under 60 characters)
- Meta descriptions (under 160 characters)
- Focus keyword per page/post
- Clean URL structure (slugs)
- Internal linking

**Technical SEO**:
- XML sitemap (auto-generated by Yoast)
- Submit to Google Search Console
- Canonical URLs
- Proper heading hierarchy
- Schema markup (Yoast handles basic schema)

### Norwegian Language Considerations

**Bokmål vs Nynorsk**: Use Bokmål (more common)

**Common terms**:
- Nyheter = News
- Arrangementer = Events
- Medlemskap = Membership
- Kontakt = Contact
- Om klubben = About the club
- Treninger = Training sessions

**Date format**: DD.MM.YYYY (Norwegian standard)
- Example: 13.03.2026

**Character encoding**: UTF-8 (supports Norwegian characters: æ, ø, å)

## Development Workflow

### Local Development (Optional)

If setting up local WordPress for testing:

**Recommended tools**:
- Local by Flywheel (easiest)
- MAMP/XAMPP
- Docker (for advanced users)

**Not required**: Can develop directly on hosting if preferred

### Deployment

**Direct to production**:
- This is a small site with low traffic
- Acceptable to make changes directly on live site
- **Always backup first** before major changes

**For major updates**:
1. Backup site (UpdraftPlus)
2. Test changes in safe environment if possible
3. Make changes during low-traffic times
4. Monitor for issues after deployment

### Version Control

**This documentation repo**:
- Commit documentation updates
- Commit content templates
- Do NOT commit WordPress core, themes, or plugins

**WordPress site**:
- Not version controlled (hosted on provider)
- Backups via UpdraftPlus serve as "versions"

## Common Tasks

### Adding a New Page

1. In WordPress: Pages → Add New
2. Copy content from `content/pages/[page-name].md`
3. Paste and format in WordPress editor
4. Add featured image
5. Set page attributes (parent, template)
6. Publish
7. Add to menu if needed (Appearance → Menus)

### Creating a News Post

1. Posts → Add New
2. Write title and content
3. Add featured image
4. Select category
5. Configure Yoast SEO
6. Publish or save draft

### Updating Theme Design

1. Appearance → Customize
2. Make changes in Customizer
3. Preview changes
4. Click "Publish"
5. Clear cache if changes don't appear

### Installing a Plugin

1. Plugins → Add New
2. Search for plugin
3. Check ratings and reviews
4. Click "Install Now"
5. Click "Activate"
6. Configure plugin settings

## Troubleshooting

### Common Issues

**White Screen of Death**:
- Disable plugins via FTP or hosting control panel
- Enable WordPress debug mode
- Check error logs
- Contact hosting support

**Can't Upload Images**:
- Check file size limits (Settings → Media)
- Increase upload limit in hosting control panel
- Check file permissions

**Site is Slow**:
- Enable caching
- Optimize images
- Disable unnecessary plugins
- Check with hosting provider

**Contact Form Not Sending**:
- Check spam folder
- Verify email settings
- Install WP Mail SMTP plugin
- Test with different email address

### Getting Help

**WordPress Documentation**: [wordpress.org/support](https://wordpress.org/support/)
**Astra Documentation**: [wpastra.com/docs](https://wpastra.com/docs/)
**WordPress Norge**: [wpnorge.no](https://wpnorge.no/)
**Hosting Support**: Contact hosting provider's support team

## Future Enhancements (Phase 2)

When ready to implement:

### Facebook Feed Integration
1. Install "Custom Facebook Feed" plugin
2. Connect to Elgane Facebook page
3. Add feed widget to homepage or sidebar
4. Configure display settings

### Calendar for Security Leaders
1. Install "The Events Calendar" plugin
2. Create custom event type: "Sikringsleder"
3. Set up recurring events
4. Add capability to assign security leader to events
5. Display calendar on relevant page

### Photo Gallery
- Use WordPress built-in gallery blocks
- Or install Envira Gallery/NextGEN Gallery
- Create separate gallery page or embed in posts

### Member Login Area (If Needed)
- Not currently planned
- Would require membership plugin (Paid Memberships Pro, etc.)
- Only implement if absolutely necessary

## Maintenance Schedule

**Weekly**:
- Check for plugin/theme updates
- Review recent posts for quality
- Monitor backup status

**Monthly**:
- Review security scan results
- Check site performance (PageSpeed)
- Update content as needed
- Review analytics (if Google Analytics installed)

**Quarterly**:
- Major WordPress updates
- Content audit
- SEO review
- Accessibility check

**Annually**:
- Renew domain and hosting
- Review and update all pages
- Major design refresh (if needed)
- Update admin guide if workflow changes

## Contact

**Project Owner**: Elgane Motorsykkelklubb
**Technical Contact**: [To be filled in]
**Content Manager**: [To be filled in]

## Notes for Claude Code

When working with this project:

1. **This is documentation, not code**: Focus on improving documentation, not writing WordPress PHP code
2. **Respect the tech stack**: WordPress is chosen for ease of use, not cutting-edge tech
3. **Keep it simple**: Solutions should be accessible to "basic technical" skill level users
4. **Norwegian context**: Remember this is a Norwegian club with Norwegian users
5. **Budget constraints**: 0-500 NOK/year budget - recommend free/cheap solutions
6. **Low traffic site**: Optimize for simplicity and maintainability, not massive scale
7. **WordPress best practices**: Follow WordPress coding standards and best practices
8. **Accessibility**: Ensure all solutions are accessible (WCAG AA minimum)
9. **Mobile-first**: Most users will access on mobile devices

## Updates

Last updated: 2026-03-13

This file should be updated when:
- Technology stack changes
- New plugins are added to essentials
- Workflow changes
- New phases are planned
- Contact information changes
