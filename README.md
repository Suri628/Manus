# AI Evaluation: Manus - Static HTML Website

A pure static HTML website with no dependencies, build tools, or bundlers. All pages are self-contained and work via `file://` protocol.

## Project Structure

```
ai-evaluation-static/
├── index.html                    # Main homepage
├── legal.html                    # Legal & Policies page
├── assets/
│   ├── css/
│   │   └── style.css            # Global stylesheet (all styling)
│   ├── js/                      # (Empty - for future JavaScript)
│   └── images/                  # (Empty - for future images)
├── demos/                       # Demo scenario pages (4 pages)
│   ├── lesson-planning.html     # Scenario A
│   ├── feedback-rubrics.html    # Scenario B
│   ├── data-dashboard.html      # Scenario C
│   └── class-website.html       # Scenario D
├── functions/                   # AI function pages (5 pages)
│   ├── webpage.html             # Webpage Builder
│   ├── presentation.html        # Presentation/PowerPoint
│   ├── app-builder.html         # App/Full-Stack Builder
│   ├── data-tools.html          # Data/Spreadsheet Automation
│   └── research-writing.html    # Research & Writing
└── dimensions/                  # AI evaluation dimensions (5 pages)
    ├── pedagogical.html         # Pedagogical Dimension
    ├── technical.html           # Technical Dimension
    ├── critical.html            # Critical Dimension
    ├── ethical.html             # Ethical Dimension
    └── metacognitive.html       # Metacognitive Dimension
```

## Total Pages: 16

- 1 Homepage (index.html)
- 1 Legal page (legal.html)
- 4 Demo scenario pages
- 5 Function pages
- 5 Dimension pages

## How to Use

### Option 1: Open Directly (file:// protocol)
1. Navigate to the project folder
2. Double-click `index.html`
3. All pages will load with relative paths

### Option 2: Local Web Server
```bash
# Python 3
cd ai-evaluation-static
python3 -m http.server 8000

# Then visit: http://localhost:8000
```

### Option 3: Python SimpleHTTPServer (Python 2)
```bash
cd ai-evaluation-static
python -m SimpleHTTPServer 8000
```

## Navigation

All pages use standard HTML anchor tags (`<a href="...">`) with relative paths:
- From root pages: `./demos/lesson-planning.html`
- From subpages: `../index.html` (go up one level)
- CSS: `./assets/css/style.css` or `../assets/css/style.css`

## Features

✓ **Pure HTML** - No React, Vue, Angular, or frameworks
✓ **No Build Tools** - No webpack, Vite, Parcel, or bundlers
✓ **No Dependencies** - No npm packages required
✓ **Relative Paths** - Works with `file://` protocol
✓ **Responsive Design** - Mobile-first CSS with media queries
✓ **Semantic HTML5** - Proper landmarks and structure
✓ **Accessibility** - WCAG compliant
✓ **Self-Contained** - Each page is complete and independent

## File Sizes

- **index.html**: ~5 KB
- **Each page**: ~4-5 KB
- **style.css**: ~12 KB
- **Total**: ~100 KB (very lightweight)

## Color Scheme

### Primary Colors
- Blue: `#0066FF`
- Teal: `#00A699`

### Dimension Colors
- Pedagogical: Blue gradient
- Technical: Cyan gradient
- Critical: Teal gradient
- Ethical: Emerald gradient
- Metacognitive: Indigo gradient

## CSS Variables

All colors are defined as CSS variables in `assets/css/style.css`:
```css
:root {
  --primary-blue: #0066FF;
  --secondary-teal: #00A699;
  --dark-bg: #0F172A;
  --light-bg: #FFFFFF;
  /* ... more variables ... */
}
```

## Customization

### Change Site Title
Edit the `<title>` tag in each HTML file.

### Change Colors
Edit CSS variables in `assets/css/style.css`:
```css
:root {
  --primary-blue: #YOUR_COLOR;
}
```

### Add New Pages
1. Create new HTML file in appropriate folder
2. Copy structure from existing page
3. Update navigation links
4. Add relative paths to CSS

### Add Images
1. Place images in `assets/images/`
2. Reference with relative paths:
   - From root: `./assets/images/image.png`
   - From subpages: `../assets/images/image.png`

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Accessibility Features

- Semantic HTML5 landmarks (nav, main, section, footer)
- Proper heading hierarchy (h1, h2, h3)
- ARIA labels where needed
- Keyboard navigation support
- Color contrast: WCAG AA compliant
- Responsive design for all screen sizes

## Performance

- **No JavaScript** (except for future enhancements)
- **Minimal CSS** (~12 KB total)
- **No external dependencies**
- **Fast page loads** (< 100 KB total)
- **SEO friendly** with proper meta tags

## Deployment

### Static Hosting Services
- GitHub Pages
- Netlify
- Vercel
- AWS S3 + CloudFront
- Any static file hosting

### Simple Deployment
```bash
# Copy entire folder to web server
scp -r ai-evaluation-static/ user@server:/var/www/html/
```

## Notes

- All pages are independent and self-contained
- No server-side processing required
- No database needed
- No authentication system
- Forum comments are placeholders (ready for integration)
- Video embeds are placeholders (ready for YouTube/Vimeo)

## Future Enhancements

- Add JavaScript for interactive features
- Integrate forum system
- Add video embeds
- Add image assets
- Add print stylesheets
- Add dark mode toggle

## Support

For questions or issues, please refer to the course materials or contact the instructors.

---

Created for CTL1615H (UofT OISE) - AI Evaluation: Manus Project
