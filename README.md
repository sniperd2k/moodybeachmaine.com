# Moody Beach Maine - The Canonicus

Oceanfront rental property website for The Canonicus, located on Moody Beach (private beach), Wells, Maine.

## Overview

This is a modern, responsive, single-page website showcasing a 3-bedroom, 1.5-bath oceanfront rental property. The site features an image gallery, rental information, directions, and contact details.

## Features

- **Responsive Design**: Mobile-first approach, works on all device sizes
- **Image Gallery**: Interactive lightbox gallery with thumbnails (lightGallery)
- **Modern HTML5**: Semantic markup with accessibility features
- **SEO Optimized**: Structured data, meta tags, Open Graph, Twitter Cards
- **Accessible**: ARIA labels, keyboard navigation, focus indicators
- **Performance**: Optimized images, lazy loading, modern CSS

## File Structure

```
moodybeachmaine.com/
├── index.html              # Main HTML page
├── css/
│   └── styles.css          # Consolidated stylesheet (CSS Grid, responsive)
├── images/                 # Gallery images (1.jpg - 15.jpg)
│   ├── 1.jpg - 15.jpg      # Property photos
│   └── background.png      # Background image
├── README.md               # This file
├── MAINTENANCE.md          # Maintenance guide
├── MODERNIZATION_PLAN.md   # Complete modernization plan
├── CHANGELOG.md            # Change history
└── [other documentation]   # Additional project docs
```

## Quick Start

### Local Development

1. **Start a local server** (required for YouTube embeds and external resources):

   **Python 3:**
   ```bash
   python3 -m http.server 8000
   ```

   **Node.js (npx serve):**
   ```bash
   npx serve -p 8000
   ```

2. **Open in browser:**
   ```
   http://localhost:8000
   ```

### Production Deployment

Simply upload all files to your web server. The site is static HTML/CSS/JS with no build process required.

**Important:** Ensure your server supports:
- Static file serving
- HTTPS (recommended for YouTube embeds and modern features)

## Dependencies

### External CDN Resources

- **lightGallery 2.7.2** (jsDelivr CDN)
  - Gallery functionality
  - Thumbnail plugin
  - CSS stylesheets

- **Google Analytics** (gtag.js)
  - Tracking ID: `G-CJP2HX87N2`

### No Local Dependencies

All JavaScript libraries are loaded via CDN. No npm, package.json, or build tools required.

## Browser Support

- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile**: iOS Safari, Chrome Mobile, Samsung Internet
- **Minimum**: Browsers supporting CSS Grid (2017+)

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Grid, Flexbox, Custom Properties (Variables)
- **JavaScript**: Vanilla JS (ES6+)
- **lightGallery**: Image gallery library
- **Schema.org**: Structured data (JSON-LD)

## Key Features Explained

### Responsive Design

- **Mobile** (< 576px): Single column layout, optimized spacing
- **Tablet** (576-768px): Adjusted layout, readable text
- **Desktop** (> 768px): Original 900px container layout

### Image Gallery

- Main image displays prominently
- Click main image or thumbnails to open lightbox
- Thumbnail navigation within lightbox
- Keyboard navigation (arrow keys, ESC to close)
- Touch gestures on mobile devices

### Accessibility

- Skip-to-content link
- ARIA labels on interactive elements
- Keyboard navigation support
- Focus indicators (3px outline)
- Semantic HTML structure
- Descriptive alt text on all images

### SEO

- Structured data (JSON-LD) for VacationRental schema
- Optimized meta tags
- Open Graph tags for social sharing
- Twitter Card tags
- Semantic heading hierarchy

## Customization

### Colors

Edit CSS variables in `css/styles.css`:

```css
:root {
  --color-primary: #0A65C9;
  --color-secondary: #686868;
  --color-text: #05060a;
  --color-background: #000;
  /* ... */
}
```

### Images

Replace images in `images/` directory:
- Maintain naming: `1.jpg` through `15.jpg`
- Recommended: 600x450px for main images, 80x60px for thumbnails
- Update alt text in `index.html` when changing images

### Content

Edit `index.html` directly:
- Update rental information in the Rental Information section
- Modify contact details in Contact Information section
- Update structured data (JSON-LD) if property details change

## Maintenance

See `MAINTENANCE.md` for detailed maintenance instructions.

## Documentation

- **MODERNIZATION_PLAN.md**: Complete modernization plan and progress
- **CHANGELOG.md**: Detailed change history
- **CURRENT_STATE.md**: Technical documentation
- **DEV_SETUP.md**: Development environment setup
- **TESTING_CHECKLIST.md**: Testing procedures

## Contact

**Property Owners**: Mandy Underwood / Jon Underwood
**Phone**: 1-603-512-2645
**Email**: amandaund@gmail.com

## License

Private property website. All rights reserved.

---

**Last Updated**: January 2025
**Website**: https://moodybeachmaine.com

