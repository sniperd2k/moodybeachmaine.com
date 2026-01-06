# Current State Documentation
## Moody Beach Maine - The Canonicus Website

**Documentation Date**: [To be completed during Phase 1]
**Purpose**: Baseline documentation before modernization

---

## Dependencies

### JavaScript Libraries
| Library | Version | Status | Purpose |
|---------|---------|--------|---------|
| jQuery | 1.2.6 | ⚠️ Deprecated | DOM manipulation, event handling |
| Galleria Plugin | 1.0 (jquery.galleria.js) | ⚠️ Old | Image gallery functionality |
| Curvy Corners | Unknown | ⚠️ Deprecated | Rounded corners effect |
| Drop Shadow Plugin | 1.6 | ⚠️ Deprecated | Drop shadow effects |
| Google Analytics | gtag.js | ✅ Current | Analytics tracking |

### CSS Frameworks
| Framework | Version | Status | Purpose |
|-----------|---------|--------|---------|
| 960 Grid System | Unknown | ⚠️ Deprecated | Layout grid system |
| Reset CSS | Unknown | ⚠️ Old | CSS reset |
| Text CSS | Unknown | ⚠️ Old | Typography |

### HTML
- **DOCTYPE**: XHTML 1.1 (⚠️ Deprecated)
- **Character Encoding**: UTF-8
- **Viewport Meta**: ❌ Missing (critical for responsive)

---

## Features Checklist

### Gallery Features
- [x] 15 images displayed as thumbnails
- [x] Main image display (600px width)
- [x] Thumbnail navigation (click to view)
- [x] Click main image to advance
- [x] Browser history support (back button)
- [x] Bookmarkable URLs
- [x] Fade transitions on image change
- [x] Thumbnail opacity effects (0.3 inactive, 1.0 active)
- [x] Hover effects on thumbnails
- [x] Image captions/titles

### Content Sections
- [x] Header: "Moody Beach" / "The Canonicus"
- [x] Property description
- [x] Rental information (8 bullet points)
- [x] Directions section with Google Maps link
- [x] YouTube video embed
- [x] Contact information (phone, email)

### Visual Effects
- [x] Rounded corners on main container
- [x] Drop shadow on h1 heading
- [x] Background image (images/background.png)
- [x] Custom color scheme (blues)

---

## File Structure

```
moodybeachmaine.com/
├── index.html (main page)
├── index.php (old/test version)
├── style.css (legacy, not used)
├── css/
│   ├── reset.css
│   ├── text.css
│   ├── 960.css
│   ├── style.css (active)
│   ├── galleria.css
│   └── uncompressed/ (backup files)
├── images/
│   ├── 1.jpg through 15.jpg (gallery images)
│   ├── background.png
│   └── old/ (archived images)
├── jquery-1.2.6.min.js
├── jquery.galleria.js
├── jquery.curvycorners.min.js
├── jquery.plugin.dropshadow.js
├── galleria-1.2.9.js (not used)
└── [other JS files]
```

---

## Browser Compatibility

### Currently Tested/Supported
- Safari 3
- Firefox 2
- MSIE 6
- MSIE 7
- Opera 9

**Note**: These are extremely outdated browsers. Modern browsers should be targeted.

---

## Content Inventory

### Gallery Images (15 total)
1. View from the road
2. Morning on the beach, high tide
3. Eat-in kitchen with dishwasher
4. View from the beach
5. Ocean side master bedroom
6. West downstairs bedroom
7. West upstairs bedroom
8. Living room
9. Upstairs full bath
10. Porch
11. Porch (second view)
12. Low tide
13. Walkway
14. Cubby storage
15. Downstairs half bath

### Text Content
- Property name: "The Canonicus"
- Location: Moody Beach (private beach), Wells, Maine
- Address: 333 Ocean Ave, Wells Maine 04090
- Property type: 3 bedroom, 1.5 bath house
- Rental period: June - October, Saturday to Saturday
- Max occupants: 6
- Contact: Mandy Underwood/Jon Underwood
- Phone: 1-603-512-2645
- Email: amandaund@gmail.com

---

## Technical Debt

### Critical Issues
1. ❌ No responsive design (fixed 900px width)
2. ❌ Uses deprecated XHTML 1.1
3. ❌ No viewport meta tag
4. ❌ jQuery 1.2.6 (security vulnerabilities)
5. ❌ Deprecated browser detection code

### Medium Priority
1. ⚠️ Inline styles in HTML
2. ⚠️ Multiple CSS files (could be consolidated)
3. ⚠️ Deprecated CSS properties
4. ⚠️ No image optimization
5. ⚠️ No lazy loading

### Low Priority
1. ℹ️ Commented-out old Google Analytics code
2. ℹ️ Unused files (index.php, style.css root, galleria-1.2.9.js)
3. ℹ️ Old image backups in /images/old/

---

## Performance Baseline

**To be measured during Phase 1**:
- Page load time
- Image file sizes
- Total page weight
- Number of HTTP requests

---

## Accessibility Status

**Current Issues**:
- ⚠️ No ARIA labels
- ⚠️ Keyboard navigation not fully supported
- ⚠️ Color contrast not verified
- ⚠️ No skip links
- ✅ Images have alt text (need to verify quality)

---

## SEO Status

**Current**:
- ✅ Meta description present
- ✅ Meta keywords present
- ✅ Canonical URL set
- ✅ Google Analytics configured
- ⚠️ No structured data
- ⚠️ Heading hierarchy needs review

---

## Notes

- Site is currently functional but uses outdated technologies
- All content and features must be preserved during modernization
- Visual appearance should remain similar but improved
- Focus on mobile experience is critical

