# Development Environment Setup
## Moody Beach Maine Website

This guide explains how to set up a local development environment for the Moody Beach Maine website.

---

## Quick Start

### Option 1: Python HTTP Server (Recommended - Simple)
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
Then open: `http://localhost:8000`

### Option 2: Node.js http-server
```bash
# Install globally (one time)
npm install -g http-server

# Run server
http-server -p 8000
```
Then open: `http://localhost:8000`

### Option 3: PHP Built-in Server
```bash
php -S localhost:8000
```
Then open: `http://localhost:8000`

### Option 4: VS Code Live Server Extension
1. Install "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"

---

## File Structure

```
moodybeachmaine.com/
├── index.html          # Main page (open this)
├── css/                # Stylesheets
├── images/             # Gallery images and assets
├── *.js                # JavaScript files
└── Documentation/      # Project documentation
```

---

## Testing Locally

### Basic Test
1. Start local server (see options above)
2. Open `http://localhost:8000` in browser
3. Verify:
   - Page loads without errors
   - All 15 gallery images display
   - Gallery navigation works
   - No console errors

### Browser DevTools Testing
- **Chrome DevTools**: F12 or Cmd+Option+I (Mac) / Ctrl+Shift+I (Windows)
- **Firefox DevTools**: F12 or Cmd+Option+I (Mac) / Ctrl+Shift+I (Windows)
- **Safari DevTools**: Enable in Preferences → Advanced → "Show Develop menu"

### Responsive Testing
Use browser DevTools device emulation:
- Mobile: 375px, 390px, 414px widths
- Tablet: 768px, 1024px widths
- Desktop: 1280px, 1920px widths

---

## Development Workflow

1. **Make Changes**: Edit HTML, CSS, or JavaScript files
2. **Test Locally**: Refresh browser to see changes
3. **Test Responsive**: Use DevTools device emulation
4. **Verify**: Check console for errors
5. **Commit**: When ready, commit changes

---

## Important Notes

- **No Build Process**: This is a static site, no compilation needed
- **Direct Editing**: Edit files directly, changes appear on refresh
- **Backup**: Always have `index.html.backup` before major changes
- **Testing**: Test in multiple browsers before deploying

---

## Troubleshooting

### Images Not Loading
- Check file paths are correct (relative paths from `index.html`)
- Verify images exist in `images/` directory
- Check browser console for 404 errors

### CSS Not Applying
- Hard refresh: Cmd+Shift+R (Mac) / Ctrl+Shift+R (Windows)
- Check CSS file paths in `<link>` tags
- Verify CSS syntax is correct

### JavaScript Errors
- Check browser console (F12)
- Verify jQuery and plugins are loaded
- Check for syntax errors in custom scripts

---

## Next Steps

After setting up local environment:
1. ✅ Verify site works locally
2. ✅ Test all gallery functionality
3. ✅ Check responsive behavior (if implemented)
4. ✅ Proceed with modernization phases

