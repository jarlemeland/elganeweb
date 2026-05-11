# Logo Files - Elgane Motorsykkelklubb

This directory should contain the official Elgane Motorsykkelklubb logo files in various formats.

## Required Logo Formats

### For WordPress Website

**Primary Logo (Header)**:
- **Format**: PNG with transparent background (preferred) or SVG
- **Size**: Width 200-400px, height proportional
- **File naming**: `elgane-logo.png` or `elgane-logo.svg`
- **Use**: Main website header logo

**Favicon**:
- **Format**: ICO or PNG
- **Size**: 512x512px (WordPress will auto-generate smaller sizes)
- **File naming**: `elgane-favicon.png`
- **Use**: Browser tab icon, bookmark icon

**Footer Logo** (optional):
- **Format**: PNG
- **Size**: Smaller version, width 100-150px
- **File naming**: `elgane-logo-footer.png`
- **Use**: Footer area if needed

### Additional Formats (Optional)

**High Resolution**:
- **Format**: PNG or PDF
- **Resolution**: 300 DPI or higher
- **File naming**: `elgane-logo-hires.png`
- **Use**: Print materials, banners, merchandise

**Dark Background Version**:
- **Format**: PNG with transparent background
- **File naming**: `elgane-logo-light.png`
- **Use**: On dark backgrounds (if logo has dark colors)

**Light Background Version**:
- **Format**: PNG with transparent background
- **File naming**: `elgane-logo-dark.png`
- **Use**: On light backgrounds

**Horizontal Version**:
- **Format**: PNG
- **File naming**: `elgane-logo-horizontal.png`
- **Use**: When wider logo is needed

**Vertical/Stacked Version**:
- **Format**: PNG
- **File naming**: `elgane-logo-vertical.png`
- **Use**: When taller/stacked logo is needed

**Icon/Symbol Only**:
- **Format**: PNG
- **Size**: Square (e.g., 500x500px)
- **File naming**: `elgane-icon.png`
- **Use**: Social media profile pictures, app icons

## File Organization

Store logo files in this directory with clear naming:

```
logo/
├── README.md (this file)
├── elgane-logo.png              # Primary logo for website
├── elgane-logo.svg              # Vector version (if available)
├── elgane-favicon.png           # Favicon (512x512px)
├── elgane-logo-hires.png        # High resolution for print
├── elgane-logo-light.png        # Version for dark backgrounds (if needed)
├── elgane-logo-dark.png         # Version for light backgrounds (if needed)
├── elgane-logo-horizontal.png   # Horizontal layout
├── elgane-logo-vertical.png     # Vertical layout
└── elgane-icon.png              # Icon/symbol only
```

## Logo Guidelines

### Colors

Ensure logo uses the official Elgane colors:
- **Primary green**: #3fb970
- **Dark elements**: #1a1a1a (if applicable)
- **White/light elements**: #ffffff (if applicable)

See `../colors.md` for complete color palette.

### Usage Guidelines

**Do**:
- ✅ Use official logo files only
- ✅ Maintain proper spacing around logo (clear space)
- ✅ Use appropriate logo version for background color
- ✅ Keep logo proportions intact
- ✅ Use high-resolution versions for print

**Don't**:
- ❌ Stretch or distort logo
- ❌ Change logo colors
- ❌ Add effects or shadows (unless part of design)
- ❌ Use low-resolution logo on large surfaces
- ❌ Place logo on busy backgrounds where it's hard to read

### WordPress Implementation

**Upload logo to WordPress**:
1. Log into WordPress admin
2. Go to **Appearance** → **Customize**
3. Click **Header Builder** → **Site Identity**
4. Click **Select Logo**
5. Upload `elgane-logo.png` or `elgane-logo.svg`
6. Adjust logo width if needed
7. Click **Publish**

**Upload favicon**:
1. Go to **Appearance** → **Customize**
2. Click **Site Identity**
3. Click **Select Site Icon**
4. Upload `elgane-favicon.png` (512x512px)
5. WordPress will crop and generate all needed sizes
6. Click **Publish**

### Creating Logo Files

If logo files need to be created or edited:

**Recommended tools**:
- **Adobe Illustrator** (professional vector editing)
- **Inkscape** (free vector editing)
- **Photoshop** (raster editing)
- **GIMP** (free raster editing)
- **Canva** (online, user-friendly)

**Tips**:
- Start with vector format (SVG/AI) when possible
- Export to PNG at appropriate sizes
- Use transparent backgrounds for PNGs
- Save high-resolution versions for future use
- Keep source files (.ai, .svg, .psd) for future editing

### Federation Logos

If adding federation logos (NMF, FIM):

**Store in subdirectory**:
```
logo/
├── federation/
│   ├── nmf-logo.png
│   └── fim-logo.png
```

**Usage**:
- Add to footer or sidebar
- Link to respective websites
- Ensure logos are official and approved for use

### Testing Logo

After uploading to WordPress, test:
- [ ] Logo displays correctly in header
- [ ] Logo is clear and sharp on desktop
- [ ] Logo is readable on mobile
- [ ] Logo works with dark/light header backgrounds
- [ ] Favicon appears in browser tab
- [ ] Logo scales properly when browser is resized

## Getting Logo Files

If logo files are not yet available:

1. **Contact club board** for existing logo files
2. **Scan/photograph** existing logos if only physical versions exist
3. **Hire designer** to create digital versions if needed
4. **Recreate in vector format** for best quality

## Updating This Directory

When adding logo files to this directory:

1. Follow naming conventions above
2. Add brief description in this README if needed
3. Update WordPress logo if main logo changes
4. Inform all admins of changes

## Questions

For questions about logo files or usage:
- Contact: [Web admin email]
- Or: Club board/leadership

---

**Last Updated**: March 2026
