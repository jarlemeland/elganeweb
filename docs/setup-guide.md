# WordPress Setup Guide - Elgane Motorsykkelklubb

This guide provides complete step-by-step instructions for setting up the Elgane website using WordPress.

## Prerequisites

Before starting, you'll need:
- Budget: 350-500 NOK/year for domain and hosting
- Email address for registration
- Payment method (credit card or Norwegian bank account)
- About 2-3 hours for initial setup

## Step 1: Domain Registration

### Option A: Register through hosting provider (Recommended)
Most hosting providers offer domain registration during signup. This is the easiest option.

### Option B: Register separately
1. Go to a Norwegian domain registrar:
   - Domeneshop.no
   - One.com
   - Loopia.no

2. Search for **elgane.no**
3. Check availability and pricing
4. Register domain (typically 150-200 NOK/year)
5. Note: You'll need to point the domain to your hosting later

## Step 2: Hosting Setup

### Recommended: One.com "Start" Plan

**Why One.com:**
- Easy WordPress installation (one-click installer)
- Norwegian customer support
- Includes email accounts
- Free SSL certificate
- Price: ~300 NOK/year

**Sign up process:**

1. Go to [one.com](https://www.one.com/no/)
2. Select "Webhotell" → "Start" plan
3. Choose billing period (1 year recommended)
4. Add domain:
   - If not registered yet: Register elgane.no through One.com
   - If already registered: Transfer or point existing domain

5. Create account:
   - Enter email address
   - Create strong password
   - Fill in club contact information

6. Complete payment
7. Wait for account activation (usually immediate)

### Alternative Hosting Providers

**Loopia "Webhotell Mini"** (~200 NOK/year):
- More budget-friendly
- Good Norwegian support
- One.click WordPress installer
- Website: [loopia.no](https://www.loopia.no/)

**Webhotell.no "Start"** (~250 NOK/year):
- Norwegian-focused provider
- Good performance
- WordPress support
- Website: [webhotell.no](https://www.webhotell.no/)

## Step 3: WordPress Installation

### Using One.com's WordPress Installer

1. **Log into your hosting control panel:**
   - Go to one.com and log in
   - Navigate to "Mitt One.com" (My One.com)

2. **Find WordPress installer:**
   - Look for "Webhosting" or "Webhotell"
   - Find "WordPress" option or "Install application"
   - Click "Install WordPress"

3. **Configure WordPress installation:**
   - **Installation directory**: Leave blank (install in root)
   - **Site name**: Elgane Motorsykkelklubb
   - **Site description**: Motorsykkelklubb i Norge - ATV, MX og Speedway
   - **Admin username**: Choose secure username (NOT "admin")
   - **Admin password**: Create strong password (save it safely!)
   - **Admin email**: Enter club's main email address
   - **Language**: Norwegian (Norsk bokmål)

4. **Start installation:**
   - Click "Install" or "Installer"
   - Wait for installation to complete (1-2 minutes)
   - Note the admin URL: typically `elgane.no/wp-admin`

5. **First login:**
   - Go to `https://elgane.no/wp-admin`
   - Log in with your admin credentials
   - You should see the WordPress dashboard

## Step 4: Basic WordPress Configuration

### General Settings

1. Go to **Innstillinger** (Settings) → **Generelt** (General)
2. Configure:
   - **Nettstedets tittel** (Site title): Elgane Motorsykkelklubb
   - **Slagord** (Tagline): Motorsykkelklubb i Norge - ATV, MX og Speedway
   - **WordPress-adresse (URL)**: https://elgane.no
   - **Nettstedsadresse (URL)**: https://elgane.no
   - **E-postadresse**: Club's main email
   - **Tidssone** (Timezone): Europe/Oslo
   - **Datoformat** (Date format): Choose Norwegian format
   - **Språk på nettstedet** (Site language): Norsk bokmål
3. Click **Lagre endringer** (Save changes)

### Permalink Settings

1. Go to **Innstillinger** → **Permalenker** (Permalinks)
2. Select **Innleggsnavn** (Post name) - this creates clean URLs
3. Click **Lagre endringer**

### Reading Settings

1. Go to **Innstillinger** → **Lesing** (Reading)
2. Configure:
   - **Hjemmesiden viser** (Homepage displays):
     - Option 1: "Siste innlegg" (Latest posts) - for news-focused homepage
     - Option 2: "En statisk side" (A static page) - for custom homepage
   - **Syndikeringsfeeder viser de siste**: 10 innlegg (posts)
3. Click **Lagre endringer**

## Step 5: Theme Installation

### Install Astra Theme

1. Go to **Utseende** (Appearance) → **Temaer** (Themes)
2. Click **Legg til nytt** (Add new)
3. Search for "Astra"
4. Find "Astra" theme by Brainstorm Force
5. Click **Installer** (Install)
6. After installation, click **Aktiver** (Activate)

### Basic Theme Configuration

1. After activation, you may see "Install Astra Starter Sites" - you can skip this
2. Go to **Utseende** → **Tilpass** (Customize)
3. This opens the WordPress Customizer
4. You'll customize the design in detail in Step 7

## Step 6: Essential Plugins Installation

### Security: Wordfence

1. Go to **Programtillegg** (Plugins) → **Legg til nytt** (Add new)
2. Search for "Wordfence Security"
3. Click **Installer nå** (Install now)
4. Click **Aktiver** (Activate)
5. Follow setup wizard:
   - Enter email for security alerts
   - Choose free version
   - Complete setup

### Backup: UpdraftPlus

1. Go to **Programtillegg** → **Legg til nytt**
2. Search for "UpdraftPlus"
3. Install and activate "UpdraftPlus WordPress Backup Plugin"
4. Go to **Innstillinger** → **UpdraftPlus-sikkerhetskopier**
5. Click **Innstillinger** (Settings) tab
6. Configure backup schedule:
   - **Filer sikkerhetskopiplan**: Ukentlig (Weekly)
   - **Database sikkerhetskopiplan**: Ukentlig (Weekly)
   - **Og behold denne mengden**: 4 (keep 4 weeks of backups)
7. Choose remote storage (free options):
   - Google Drive (recommended)
   - Dropbox
   - Or "E-post" (Email) for small sites
8. Click **Lagre endringer**
9. Authenticate with your chosen cloud storage
10. Click **Sikkerhetskopier nå** (Backup now) to create first backup

### SEO: Yoast SEO

1. Go to **Programtillegg** → **Legg til nytt**
2. Search for "Yoast SEO"
3. Install and activate "Yoast SEO"
4. Follow configuration wizard:
   - Site type: "Other non-profit organization"
   - Organization name: Elgane Motorsykkelklubb
   - Upload logo if available
   - Complete wizard

### Contact Form: Contact Form 7

1. Go to **Programtillegg** → **Legg til nytt**
2. Search for "Contact Form 7"
3. Install and activate
4. Go to **Kontakt** (Contact) in admin menu
5. A default contact form is already created
6. Edit form to translate to Norwegian (or keep for now)

## Step 7: Theme Customization

See the detailed [Theme Customization Guide](theme-customization.md) for complete design setup.

Quick steps:

1. Go to **Utseende** → **Tilpass** (Customize)
2. **Global** → **Colors**:
   - Set primary color to #3fb970 (Elgane green)
   - Set heading color to match brand
3. **Header Builder**:
   - Add logo
   - Configure navigation menu
   - Set dark background color
4. **Footer Builder**:
   - Add footer content
   - Add footer menu
5. Click **Publiser** (Publish) to save changes

## Step 8: Create Page Structure

### Create Main Pages

1. Go to **Sider** (Pages) → **Legg til ny** (Add new)

2. **Create these pages:**

   **a) ATV og Sidecar**
   - Title: ATV og Sidecar
   - Add content about ATV and Sidecar branch
   - Click **Publiser** (Publish)

   **b) MX**
   - Title: MX
   - Add content about Motocross branch
   - Click **Publiser**

   **c) Speedway**
   - Title: Speedway
   - Add content about Speedway branch
   - Click **Publiser**

   **d) Om klubben** (About the club)
   - Title: Om klubben
   - Add club information, history, board members
   - Click **Publiser**

   **e) Kontakt** (Contact)
   - Title: Kontakt
   - Add contact information
   - Insert contact form: Add block → search "Contact Form 7" → insert
   - Click **Publiser**

   **f) Bane og kart** (Track and maps)
   - Title: Bane og kart
   - Add track information and Google Maps embed
   - Click **Publiser**

3. **Optional: Create custom homepage**
   - Title: Hjem
   - Design homepage layout
   - Go to **Innstillinger** → **Lesing**
   - Set "Hjemmesiden viser" to "En statisk side"
   - Choose "Hjem" as homepage
   - Optionally set a "Innleggsside" (Posts page) for news archive

### Create Navigation Menu

1. Go to **Utseende** → **Menyer** (Menus)
2. Click **opprett en ny meny** (create a new menu)
3. Name it "Hovedmeny" (Main menu)
4. Check **Hovedmeny** (Primary menu) under "Display location"
5. Add pages to menu:
   - Hjem (if static homepage) or skip
   - ATV og Sidecar
   - MX
   - Speedway
   - Om klubben
   - Kontakt
6. Drag to reorder pages
7. Click **Lagre meny** (Save menu)

### Create Footer Menu (Optional)

1. Create another menu named "Bunntekstmeny" (Footer menu)
2. Add pages:
   - Bane og kart
   - Personvern (create privacy policy page first)
3. Assign to footer location
4. Click **Lagre meny**

## Step 9: Create Initial Content

### Create News Categories

1. Go to **Innlegg** (Posts) → **Kategorier** (Categories)
2. Create categories:
   - Nyheter (News)
   - ATV & Sidecar
   - MX
   - Speedway
   - Arrangementer (Events)

### Create First News Posts

1. Go to **Innlegg** → **Legg til ny**
2. Create 2-3 initial news posts
3. For each post:
   - Add title
   - Add content
   - Set featured image (if available)
   - Select category
   - Click **Publiser**

## Step 10: Security Hardening

### Update Everything

1. Go to **Kontrollpanel** (Dashboard) → **Oppdateringer** (Updates)
2. Update WordPress core if needed
3. Update all plugins
4. Update theme

### Configure Wordfence

1. Go to **Wordfence** → **All Options**
2. Enable:
   - Two-factor authentication for admin accounts
   - Email alerts for security events
   - Login security features
3. Run first scan: **Wordfence** → **Scan**

### User Security

1. Go to **Brukere** (Users)
2. Delete default "admin" user if it exists
3. Ensure all users have strong passwords
4. Set appropriate user roles (only give "Administrator" to trusted people)

### File Permissions

1. Create/edit wp-config.php security keys (usually done automatically)
2. Consider adding to wp-config.php:
   ```php
   define('DISALLOW_FILE_EDIT', true);
   ```
   This prevents theme/plugin editing through admin panel

## Step 11: SEO Configuration

### Configure Yoast SEO

1. Go to **SEO** → **Generelt** (General)
2. Review configuration
3. Go to **SEO** → **Utseende i søk** (Search appearance)
4. Configure:
   - **Generelt**: Set site title and description
   - **Innholdstyper** (Content types): Configure how posts and pages appear
   - **Medier** (Media): Set to "Ja" (Yes) for redirecting attachment URLs

### Submit to Search Engines

1. Go to **SEO** → **Generelt** → **Webmaster Tools**
2. Add site to:
   - Google Search Console
   - Bing Webmaster Tools (optional)
3. Follow verification steps

### Create XML Sitemap

1. Yoast creates this automatically
2. View at: `https://elgane.no/sitemap_index.xml`
3. Submit to Google Search Console

## Step 12: Performance Optimization

### Enable Caching

Many hosting providers include caching. Check with your provider.

Alternative: Install a caching plugin (if needed):
1. Go to **Programtillegg** → **Legg til nytt**
2. Search for "WP Super Cache" or "W3 Total Cache"
3. Install and activate
4. Follow plugin setup wizard

### Image Optimization

1. Install "Smush" plugin (free image compression)
2. Go to **Programtillegg** → **Legg til nytt**
3. Search for "Smush"
4. Install and activate
5. Bulk compress existing images
6. Enable automatic compression for new uploads

### Test Performance

1. Go to [Google PageSpeed Insights](https://pagespeed.web.dev/)
2. Enter your domain: elgane.no
3. Review performance score
4. Aim for 70+ on mobile and desktop

## Step 13: Final Checks

### Functionality Testing

- [ ] Can you log into WordPress admin?
- [ ] Can you create and edit pages?
- [ ] Can you create and edit posts?
- [ ] Do images upload correctly?
- [ ] Does the contact form send emails?
- [ ] Do all menu links work?
- [ ] Is HTTPS working (green padlock in browser)?

### Responsive Testing

- [ ] Test on desktop browser
- [ ] Test on tablet (or resize browser)
- [ ] Test on mobile phone
- [ ] Check that navigation menu works on mobile

### Security Checks

- [ ] Is Wordfence active and configured?
- [ ] Is backup running automatically?
- [ ] Are all plugins and WordPress up to date?
- [ ] Are there any security warnings?

## Step 14: Create Admin Accounts

### Add Content Managers

1. Go to **Brukere** → **Legg til ny**
2. For each admin:
   - Fill in name and email
   - Username: use real name or club role
   - Send notification email (they'll set their password)
   - Role: **Redaktør** (Editor) for content managers
   - Role: **Administrator** only for technical admins
3. Click **Legg til ny bruker**

## Congratulations!

Your WordPress site is now set up and ready for content. Next steps:

1. Review the [Theme Customization Guide](theme-customization.md) for design refinements
2. Share the [Admin Guide](admin-guide.md) with content managers
3. Start migrating content from the old site
4. Consider Phase 2 features (Facebook feed, calendar)

## Troubleshooting

### "White screen of death"
- Disable all plugins via FTP or hosting control panel
- Enable plugins one by one to find the problem
- Contact hosting support

### Can't log in
- Use "Lost your password?" link
- Check email for reset link
- Contact hosting support if needed

### Images won't upload
- Check file size (max usually 2-8 MB)
- Check file format (JPG, PNG, GIF)
- Increase upload limit in hosting control panel

### Contact form not sending emails
- Check spam folder
- Verify email settings in hosting control panel
- Install WP Mail SMTP plugin for better email delivery

### Site is slow
- Enable caching plugin
- Optimize images with Smush
- Contact hosting support
- Consider upgrading hosting plan if traffic increases

## Getting Help

- **WordPress.org Documentation**: [wordpress.org/support](https://wordpress.org/support/)
- **WordPress Norge**: [wpnorge.no](https://wpnorge.no/) - Norwegian WordPress community
- **Hosting Support**: Contact your hosting provider's support team
- **Theme Documentation**: [wpastra.com/docs/](https://wpastra.com/docs/)
