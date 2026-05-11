# Theme Customization Guide - Elgane Motorsykkelklubb

This guide explains how to customize the Astra theme to match Elgane's branding and design requirements.

## Design Requirements

Based on the current IdrettenOnline site analysis:
- **Color scheme**: Dark navigation with green accent (#3fb970)
- **Style**: Modern, clean, professional
- **Logo**: Elgane Motorsykkelklubb logo
- **Responsive**: Must work on mobile, tablet, desktop
- **Typography**: Clean, readable fonts
- **Images**: Federation logos (NMF, FIM)

## Accessing Theme Customizer

1. Log into WordPress admin
2. Go to **Utseende** (Appearance) → **Tilpass** (Customize)
3. This opens the live customizer where you can preview changes

**Important**: Click "Publiser" (Publish) to save your changes!

## Color Scheme Setup

### Primary Color (Elgane Green)

1. In Customizer, go to **Global** → **Colors**
2. Find **Theme Color** or **Accent Color**
3. Click the color picker
4. Enter: `#3fb970` (Elgane green)
5. This color will be used for:
   - Links
   - Buttons
   - Hover states
   - Accents

### Additional Colors

**Link Color**:
- Set to `#3fb970` (same as primary)

**Heading Color**:
- Set to `#1a1a1a` (dark gray, almost black)
- Or use pure black `#000000`

**Text Color**:
- Set to `#333333` (dark gray for readability)

**Background Colors**:
- **Base Background**: `#ffffff` (white)
- **Content Background**: `#ffffff` (white)

### Header Colors

1. Go to **Header Builder** → **Header**
2. Click on the header row you want to style
3. Set colors:
   - **Background Color**: `#1a1a1a` or `#2d2d2d` (dark gray/black)
   - **Link Color**: `#ffffff` (white)
   - **Link Hover Color**: `#3fb970` (green)

## Logo Setup

### Upload Logo

1. In Customizer, go to **Header Builder**
2. Click **Site Identity** or **Logo**
3. Click **Select Logo**
4. Upload your logo file (PNG or SVG recommended)
5. Recommended dimensions:
   - Height: 50-80px
   - Width: Auto (maintain proportions)
   - Transparent background (PNG)

### Logo Settings

**Logo Width**:
- Desktop: 150-200px
- Mobile: 100-150px

**Logo Position**:
- Left-aligned (standard)

**Site Title**:
- Hide site title if logo includes text
- Or display alongside logo if logo is icon only

## Typography

### Font Selection

Astra works well with Google Fonts.

**Recommended fonts for motorsport club:**

**Headings**:
- Montserrat (modern, bold)
- Roboto (clean, professional)
- Open Sans (friendly, readable)

**Body Text**:
- Roboto (if different from headings)
- Open Sans
- Lato

### Configure Typography

1. Go to **Global** → **Typography**

2. **Base Typography** (body text):
   - **Font Family**: Open Sans or Roboto
   - **Font Weight**: 400 (regular)
   - **Font Size**: 16px
   - **Line Height**: 1.6

3. **Headings** (H1-H6):
   - **Font Family**: Montserrat or Roboto
   - **Font Weight**: 600-700 (semi-bold to bold)
   - **Font Sizes**:
     - H1: 36-42px
     - H2: 30-36px
     - H3: 24-28px
     - H4: 20-24px
     - H5: 18-20px
     - H6: 16-18px

## Header Builder Configuration

### Header Layout

Astra's Header Builder allows drag-and-drop customization.

1. Go to **Header Builder**
2. You'll see header rows: Above Header, Primary Header, Below Header

**Recommended layout:**

**Primary Header Row**:
- Left: Logo
- Center: (empty or tagline)
- Right: Primary Menu

### Desktop Header

1. Click on **Primary Header** row
2. Configure:
   - **Background Color**: `#1a1a1a` (dark)
   - **Height**: 80-100px
   - **Padding**: 15-20px top/bottom

3. **Add Logo** (if not already added):
   - Drag "Site Identity" element to left section
   - Configure logo as described above

4. **Add Menu**:
   - Drag "Primary Menu" element to right section
   - Configure menu styling below

### Mobile Header

1. Switch to mobile view (click phone icon in customizer)
2. **Mobile Header**:
   - Show mobile menu toggle (hamburger icon)
   - Logo position: Left or center
   - Toggle position: Right

3. **Mobile Menu**:
   - Dropdown style or full-screen overlay
   - Background: `#1a1a1a`
   - Links: White text
   - Hover: Green `#3fb970`

## Menu Styling

### Primary Menu (Desktop)

1. In Header Builder, click on **Primary Menu** element
2. Configure:
   - **Menu Layout**: Horizontal
   - **Submenu Type**: Dropdown
   - **Font Size**: 14-16px
   - **Font Weight**: 500-600
   - **Letter Spacing**: 0.5px
   - **Text Transform**: None or Uppercase (club preference)

3. **Menu Colors**:
   - **Link Color**: `#ffffff` (white)
   - **Link Hover Color**: `#3fb970` (green)
   - **Active Link Color**: `#3fb970` (green)
   - **Submenu Background**: `#2d2d2d` (slightly lighter dark)
   - **Submenu Link Color**: `#ffffff`

4. **Spacing**:
   - **Menu Item Spacing**: 20-30px between items
   - **Menu Item Padding**: 10-15px top/bottom

### Mobile Menu

1. In Header Builder, configure **Mobile Menu** element
2. Set:
   - **Menu Style**: Slide-in drawer or dropdown
   - **Background**: `#1a1a1a`
   - **Link Color**: `#ffffff`
   - **Divider Color**: `#3fb970` or subtle gray

## Footer Configuration

### Footer Layout

1. Go to **Footer Builder**
2. Choose layout:
   - **Simple**: Single row, centered
   - **Advanced**: Multiple columns

**Recommended layout:**

**Footer Row 1** (Main footer):
- Column 1: Club information
- Column 2: Quick links (footer menu)
- Column 3: Social media or contact info

**Footer Row 2** (Bottom footer):
- Copyright text

### Footer Styling

1. Click on footer row to configure
2. Set:
   - **Background**: `#1a1a1a` (dark, matching header)
   - **Text Color**: `#cccccc` (light gray)
   - **Link Color**: `#ffffff`
   - **Link Hover**: `#3fb970` (green)
   - **Padding**: 40-60px top/bottom

### Footer Widgets

1. **Add HTML/Text widget**:
   - Go to **Appearance** → **Widgets**
   - Find "Footer Bar Section"
   - Add "Text" or "HTML" widget
   - Enter club information

2. **Add Menu widget**:
   - Add "Navigation Menu" widget
   - Select footer menu

3. **Add Social Icons** (if available):
   - Add social media widget or HTML with links

### Copyright Section

1. In Footer Builder, click **Footer Bar** or bottom row
2. Add text:
   ```
   © 2026 Elgane Motorsykkelklubb. Alle rettigheter reservert.
   ```
3. Align center
4. Font size: 12-14px
5. Background: Darker than main footer or same

## Blog/News Layout

### Blog Archive Layout

1. Go to **Blog** → **Blog/Archive**
2. Configure:
   - **Layout**: Grid (2-3 columns) or list
   - **Post Structure**:
     - Featured image
     - Title
     - Meta (date, category)
     - Excerpt (150-200 characters)
     - Read more link

3. **Blog Grid**:
   - **Columns**: 2 on desktop, 1 on mobile
   - **Columns Gap**: 30-40px
   - **Image Position**: Top
   - **Image Ratio**: 16:9 or 4:3

### Single Post Layout

1. Go to **Blog** → **Single Post**
2. Configure:
   - **Layout**: Default or narrow (for better readability)
   - **Sidebar**: Right sidebar or no sidebar
   - **Content Width**: 750-850px (without sidebar)

3. **Post Structure**:
   - Featured image (top)
   - Title
   - Meta (date, author, category)
   - Content
   - Tags (bottom)

### Post Meta

1. Configure which meta elements to show:
   - ✅ Date
   - ✅ Category
   - ❌ Author (optional, if multiple authors)
   - ❌ Comments (if not using comments)
   - ✅ Tags

## Sidebar Configuration

### Sidebar Layout

1. Go to **Sidebar** in customizer
2. Choose layout for different page types:
   - **Homepage**: No sidebar (full-width)
   - **Blog archive**: Right sidebar
   - **Single post**: Right sidebar or no sidebar
   - **Pages**: No sidebar

### Sidebar Widgets

1. Go to **Appearance** → **Widgets**
2. Find "Primary Sidebar"
3. Add useful widgets:
   - **Categories**: Show post categories
   - **Recent Posts**: Latest 5 posts
   - **Search**: Site search
   - **Facebook Feed** (when plugin installed)
   - **Calendar** (when plugin installed)

## Homepage Design

### Option 1: Blog Homepage (Latest News)

**Best for**: News-focused sites

1. Go to **Settings** → **Reading**
2. Select "Your latest posts"
3. Posts automatically display on homepage
4. Use blog grid layout for attractive display

### Option 2: Custom Static Homepage

**Best for**: More control over layout

1. Create a new page: "Hjem" (Home)
2. Use page builder or blocks to create:
   - Hero section with club image
   - Welcome text
   - Latest news section (using "Latest Posts" block)
   - Branch sections (ATV/MX/Speedway)
   - Call-to-action (Join club, contact, etc.)

3. Go to **Settings** → **Reading**
4. Select "A static page"
5. Homepage: Hjem
6. Posts page: Create "Nyheter" page

## Responsive Design

### Mobile Optimization

1. **Use Customizer mobile preview**:
   - Click phone/tablet icons at bottom
   - Preview changes on different devices

2. **Mobile-specific settings**:
   - Font sizes: Smaller than desktop (14-16px body)
   - Padding: Reduce padding on mobile
   - Menu: Ensure mobile menu works
   - Images: Ensure images scale properly

3. **Test on real devices**:
   - iPhone/Android phone
   - iPad/Android tablet
   - Different screen sizes

### Breakpoints

Astra's responsive breakpoints:
- **Mobile**: < 768px
- **Tablet**: 768px - 991px
- **Desktop**: > 992px

## Additional Customizations

### Buttons

1. Go to **Global** → **Buttons**
2. Configure:
   - **Button Color**: `#3fb970` (green)
   - **Text Color**: `#ffffff` (white)
   - **Hover Color**: Darker green `#35a060`
   - **Border Radius**: 4px (slight rounding) or 0px (square)
   - **Padding**: 12px horizontal, 8px vertical

### Containers

1. Go to **Global** → **Container**
2. Set:
   - **Container Width**: 1200-1400px
   - **Container Padding**: 20-30px

### Spacing

1. Configure consistent spacing throughout:
   - Section padding: 60-80px top/bottom
   - Element margins: 20-30px
   - Content padding: 15-20px

## Federation Logos

### Add Logos to Footer

1. **Create HTML widget**:
   - Go to **Appearance** → **Widgets**
   - Add "Custom HTML" to footer
   - Add HTML:
     ```html
     <div class="federation-logos">
       <img src="URL-to-NMF-logo" alt="NMF - Norges Motorsportforbund" width="100">
       <img src="URL-to-FIM-logo" alt="FIM - Fédération Internationale de Motocyclisme" width="100">
     </div>
     ```

2. **Style with CSS** (see CSS section below)

### Add Logos to Sidebar or Pages

Use same approach with Image blocks or HTML.

## Custom CSS

For advanced customization, add custom CSS:

1. Go to **Additional CSS** in Customizer
2. Add CSS code

**Useful custom CSS:**

```css
/* Federation logos styling */
.federation-logos {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  margin: 20px 0;
}

.federation-logos img {
  max-width: 100px;
  height: auto;
  opacity: 0.8;
  transition: opacity 0.3s;
}

.federation-logos img:hover {
  opacity: 1;
}

/* Green accent on hover for links in content */
.entry-content a:hover {
  color: #3fb970;
}

/* Style for news category badges */
.cat-links a {
  background: #3fb970;
  color: white;
  padding: 4px 12px;
  border-radius: 3px;
  text-decoration: none;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

/* Responsive footer columns on mobile */
@media (max-width: 768px) {
  .footer-widget-area {
    text-align: center;
  }
}

/* Improve readability of post content */
.entry-content p {
  margin-bottom: 1.5em;
  line-height: 1.7;
}

/* Style for main CTA buttons */
.wp-block-button__link {
  background-color: #3fb970 !important;
  border-radius: 4px;
  padding: 12px 30px;
  font-weight: 600;
}

.wp-block-button__link:hover {
  background-color: #35a060 !important;
}
```

## Performance Optimization

### Image Settings

1. **Featured Image Size**:
   - Go to **Settings** → **Media**
   - Thumbnail: 150x150
   - Medium: 600x400 (for blog grids)
   - Large: 1200x800 (for featured images)

2. **Install Smush plugin** for automatic image optimization

### Lazy Loading

Lazy loading is built into WordPress 5.5+. Images load as users scroll.

### Font Loading

1. In Astra settings, consider:
   - Limit Google Font weights (only load needed weights)
   - Use system fonts for better performance (optional)

## Testing Checklist

After customization, test:

### Visual Testing
- [ ] Logo displays correctly on all devices
- [ ] Colors match branding (#3fb970 green)
- [ ] Fonts are readable
- [ ] Header looks good
- [ ] Footer is complete
- [ ] Menu works on desktop
- [ ] Mobile menu works
- [ ] Blog/news layout is attractive

### Functionality Testing
- [ ] All menu links work
- [ ] Images load correctly
- [ ] Forms work (contact form)
- [ ] Sidebar widgets display
- [ ] Footer widgets display
- [ ] Search works
- [ ] RSS feed works

### Responsive Testing
- [ ] Test on iPhone/Android
- [ ] Test on iPad/tablet
- [ ] Test on laptop
- [ ] Test on large desktop
- [ ] Mobile menu toggles properly
- [ ] Images scale correctly
- [ ] Text is readable on all devices

### Performance Testing
- [ ] Page loads in < 3 seconds
- [ ] Images are optimized
- [ ] No broken links
- [ ] No console errors

## Maintenance

### Regular Updates

- Update Astra theme when updates available
- Test site after theme updates
- Keep backups before major changes

### Seasonal Changes

Consider changing:
- Homepage hero image (seasonal photos)
- Colors for special events (optional)
- Featured news posts

## Advanced: Page Builder Option

For more advanced layouts, consider:
- **Elementor** (free page builder plugin)
- Works with Astra
- Drag-and-drop design
- Pre-made templates

Only install if needed for complex layouts.

## Getting Help

- **Astra Documentation**: [wpastra.com/docs/](https://wpastra.com/docs/)
- **Astra Support**: Available for pro users
- **WordPress Community**: [wordpress.org/support/](https://wordpress.org/support/)

## Next Steps

After theme customization:
1. Create all main pages (see content/pages/)
2. Add initial news posts
3. Configure menus
4. Add widgets
5. Test thoroughly
6. Launch site!
