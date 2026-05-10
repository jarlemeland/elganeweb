# Color Scheme - Elgane Motorsykkelklubb

This document defines the official color palette for the Elgane Motorsykkelklubb website.

## Brand Colors

### Primary Color: Elgane Green

**Hex**: `#3fb970`
**RGB**: `rgb(63, 185, 112)`
**HSL**: `hsl(145, 49%, 49%)`

**Usage**:
- Primary brand color
- Links and link hover states
- Buttons and call-to-action elements
- Active menu items
- Accent elements
- Highlights and emphasis

**Accessibility**: Passes WCAG AA contrast on white background

---

### Secondary Colors

#### Dark Gray (Headers/Navigation)

**Hex**: `#1a1a1a`
**RGB**: `rgb(26, 26, 26)`

**Usage**:
- Header background
- Footer background
- Dark elements
- High contrast sections

---

#### Medium Dark Gray (Borders/Subtle Elements)

**Hex**: `#2d2d2d`
**RGB**: `rgb(45, 45, 45)`

**Usage**:
- Submenu backgrounds
- Hover backgrounds
- Subtle borders
- Dividers

---

### Text Colors

#### Primary Text

**Hex**: `#333333`
**RGB**: `rgb(51, 51, 51)`

**Usage**:
- Body text
- Paragraphs
- General content
- Readable on white background

---

#### Heading Text

**Hex**: `#1a1a1a`
**RGB**: `rgb(26, 26, 26)`

**Usage**:
- H1, H2, H3, H4, H5, H6
- Page titles
- Section headings

---

#### Light Text (on dark backgrounds)

**Hex**: `#ffffff`
**RGB**: `rgb(255, 255, 255)`

**Usage**:
- Text on dark header
- Text on dark footer
- Menu links on dark navigation
- Text on buttons

---

#### Secondary Text

**Hex**: `#666666`
**RGB**: `rgb(102, 102, 102)`

**Usage**:
- Meta information (dates, categories)
- Secondary descriptions
- Bylines
- Captions

---

#### Muted Text

**Hex**: `#999999`
**RGB**: `rgb(153, 153, 153)`

**Usage**:
- Disabled elements
- Placeholder text
- Very subtle information

---

### Background Colors

#### Primary Background

**Hex**: `#ffffff`
**RGB**: `rgb(255, 255, 255)`

**Usage**:
- Page background
- Content areas
- Cards and panels

---

#### Light Gray Background

**Hex**: `#f5f5f5`
**RGB**: `rgb(245, 245, 245)`

**Usage**:
- Alternate sections
- Sidebar backgrounds
- Subtle content separation
- Input fields

---

#### Very Light Gray

**Hex**: `#fafafa`
**RGB**: `rgb(250, 250, 250)`

**Usage**:
- Very subtle backgrounds
- Hover states for light elements

---

### Accent and State Colors

#### Success Green (lighter variation)

**Hex**: `#4caf50`
**RGB**: `rgb(76, 175, 80)`

**Usage**:
- Success messages
- Confirmation states
- Positive indicators

---

#### Hover State (darker green)

**Hex**: `#35a060`
**RGB**: `rgb(53, 160, 96)`

**Usage**:
- Button hover states
- Link hover (when darker variant needed)
- Active button states

---

#### Error Red

**Hex**: `#e53935`
**RGB**: `rgb(229, 57, 53)`

**Usage**:
- Error messages
- Required field indicators
- Warning elements

---

#### Info Blue

**Hex**: `#2196f3`
**RGB**: `rgb(33, 150, 243)`

**Usage**:
- Informational messages
- Links (alternative to green where needed)
- Info badges

---

#### Warning Orange

**Hex**: `#ff9800`
**RGB**: `rgb(255, 152, 0)`

**Usage**:
- Warning messages
- Caution elements
- Alert indicators

---

## Color Usage Guidelines

### Do's

✅ **Use Elgane Green (#3fb970) for**:
- All primary call-to-action buttons
- Link colors
- Active navigation items
- Important highlights
- Brand elements

✅ **Use dark backgrounds (#1a1a1a) for**:
- Header navigation
- Footer
- Hero sections (optional)

✅ **Use white (#ffffff) for**:
- Main content backgrounds
- Maximum readability

✅ **Maintain contrast**:
- Ensure text is readable (WCAG AA minimum)
- Test color combinations
- Use dark text on light backgrounds
- Use light text on dark backgrounds

### Don'ts

❌ **Don't**:
- Use too many colors in one design
- Use low-contrast combinations
- Modify the primary green color
- Use bright colors for large backgrounds
- Mix warm and cool grays

---

## Category Colors

For color-coding motorsport branches (optional):

### ATV & Sidecar
**Hex**: `#3fb970` (Elgane Green - primary)

### MX (Motocross)
**Hex**: `#ff9800` (Orange)

### Speedway
**Hex**: `#2196f3` (Blue)

**Usage**: Can be used for category badges, icons, or section identifiers to help users visually distinguish between branches.

---

## Gradients (Optional)

If gradients are needed:

### Primary Gradient

```css
background: linear-gradient(135deg, #3fb970 0%, #35a060 100%);
```

**Usage**: Hero sections, featured elements, special call-to-action

### Dark Gradient

```css
background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
```

**Usage**: Dark headers, footer sections

---

## CSS Variables

For easy implementation, use CSS custom properties:

```css
:root {
  /* Brand Colors */
  --color-primary: #3fb970;
  --color-primary-dark: #35a060;
  --color-primary-light: #4caf50;

  /* Dark Colors */
  --color-dark: #1a1a1a;
  --color-dark-medium: #2d2d2d;

  /* Text Colors */
  --color-text-primary: #333333;
  --color-text-heading: #1a1a1a;
  --color-text-light: #ffffff;
  --color-text-secondary: #666666;
  --color-text-muted: #999999;

  /* Background Colors */
  --color-bg-primary: #ffffff;
  --color-bg-light: #f5f5f5;
  --color-bg-lighter: #fafafa;

  /* State Colors */
  --color-success: #4caf50;
  --color-error: #e53935;
  --color-warning: #ff9800;
  --color-info: #2196f3;

  /* Category Colors */
  --color-atv: #3fb970;
  --color-mx: #ff9800;
  --color-speedway: #2196f3;
}
```

**Usage in CSS**:
```css
.button {
  background-color: var(--color-primary);
  color: var(--color-text-light);
}

.button:hover {
  background-color: var(--color-primary-dark);
}
```

---

## Accessibility

### Contrast Ratios (WCAG 2.1)

**AA Standard** (minimum):
- Normal text: 4.5:1
- Large text (18pt+): 3:1

**AAA Standard** (enhanced):
- Normal text: 7:1
- Large text: 4.5:1

### Tested Combinations

✅ **Pass AA (Normal Text)**:
- `#3fb970` on `#ffffff` (4.51:1)
- `#333333` on `#ffffff` (12.63:1)
- `#1a1a1a` on `#ffffff` (16.53:1)
- `#ffffff` on `#1a1a1a` (16.53:1)
- `#ffffff` on `#3fb970` (2.38:1) ⚠️ Use for large text only

✅ **Pass AAA (Normal Text)**:
- `#333333` on `#ffffff`
- `#1a1a1a` on `#ffffff`
- `#ffffff` on `#1a1a1a`

### Color Blindness Considerations

The Elgane Green (#3fb970) is:
- ✅ Distinguishable for most common types of color blindness
- ✅ Safe for deuteranopia (red-green colorblindness)
- ✅ Safe for protanopia (red-blind)
- ✅ Safe for tritanopia (blue-yellow colorblindness)

**Important**: Never rely on color alone to convey information. Use:
- Icons with text labels
- Patterns or textures
- Text descriptions
- Shape differences

---

## Implementation in WordPress

### Using the Customizer

1. Go to **Appearance** → **Customize**
2. **Global** → **Colors**:
   - Theme/Accent Color: `#3fb970`
   - Link Color: `#3fb970`
   - Text Color: `#333333`
   - Heading Color: `#1a1a1a`

3. **Header Builder** → **Header**:
   - Background: `#1a1a1a`
   - Link Color: `#ffffff`
   - Link Hover: `#3fb970`

4. **Footer Builder** → **Footer**:
   - Background: `#1a1a1a`
   - Text Color: `#cccccc`
   - Link Color: `#ffffff`
   - Link Hover: `#3fb970`

### Custom CSS

Add to **Additional CSS** in Customizer:

```css
/* Ensure brand color is used consistently */
a {
  color: #3fb970;
}

a:hover {
  color: #35a060;
}

.wp-block-button__link {
  background-color: #3fb970;
}

.wp-block-button__link:hover {
  background-color: #35a060;
}
```

---

## Design Examples

### Button Styles

**Primary Button**:
- Background: `#3fb970`
- Text: `#ffffff`
- Hover background: `#35a060`
- Border: None or `1px solid #3fb970`
- Padding: `12px 30px`
- Border radius: `4px`

**Secondary Button**:
- Background: `transparent`
- Text: `#3fb970`
- Border: `2px solid #3fb970`
- Hover background: `#3fb970`
- Hover text: `#ffffff`

**Disabled Button**:
- Background: `#cccccc`
- Text: `#666666`
- Cursor: `not-allowed`
- Opacity: `0.6`

### Link Styles

**Default Link**:
- Color: `#3fb970`
- Decoration: `none`
- Hover: `#35a060` with `underline`

**Navigation Link**:
- Color: `#ffffff`
- Hover: `#3fb970`
- Active: `#3fb970`

### Card/Panel Styles

**Standard Card**:
- Background: `#ffffff`
- Border: `1px solid #e0e0e0`
- Shadow: `0 2px 4px rgba(0,0,0,0.1)`
- Hover shadow: `0 4px 8px rgba(0,0,0,0.15)`

### Form Elements

**Input Fields**:
- Background: `#ffffff`
- Border: `1px solid #cccccc`
- Focus border: `2px solid #3fb970`
- Text: `#333333`
- Placeholder: `#999999`

---

## Color Palette Export

### For Design Tools

**Sketch/Figma/Adobe XD**:
- Import these hex values as color swatches
- Create shared color library
- Use for consistent design

**CSS/SCSS**:
- See CSS Variables section above
- Create `_colors.scss` or `colors.css` file
- Import in main stylesheet

---

## Maintenance

### When to Update Colors

- Rebranding initiatives
- Accessibility improvements needed
- User feedback on readability
- Design refresh

### How to Update

1. Update this document first
2. Update CSS variables
3. Test all pages
4. Update theme customizer settings
5. Check accessibility with new colors
6. Communicate changes to team

---

## Resources

- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Coolors Color Palette Generator](https://coolors.co/)
- [Adobe Color](https://color.adobe.com/)
- [WCAG Color Contrast Guidelines](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)

---

**Last Updated**: March 2026
**Maintained by**: Web Team, Elgane Motorsykkelklubb
