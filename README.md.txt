# Island Title Research — Website

**Live:** https://islandtitleresearch.com  
**Stack:** Plain HTML/CSS/JS · Netlify hosting · GitHub Pages compatible

## Project Structure

```
islandtitleresearch-web/
├── index.html        # Full one-page site (self-contained)
└── README.md
```

## Hero Image

The hero background references **iStock photo ID 1022617938** (credit: Mark Zhu — Old San Juan coastline).  
To embed for production, replace the `url(...)` in `.hero-bg` with a base64 data URI:

```css
.hero-bg {
  background: linear-gradient(...), url('data:image/jpeg;base64,...') center/cover;
}
```

Or place the purchased image at `/images/hero-san-juan.jpg` and update the CSS path.

## About Photo

Replace the SVG placeholder in `#about .about-img-frame` with:
```html
<img src="images/clarissa-maldonado.jpg" alt="Clarissa S. Maldonado" style="width:100%;height:100%;object-fit:cover;" />
```

## Contact Form

The form uses `data-netlify="true"` for zero-config Netlify Forms submission.  
If deploying to GitHub Pages instead, replace with Formspree or EmailJS.

## Local Development

Open `index.html` directly in any browser — no build step required.

## Deployment

```bash
git add .
git commit -m "Update site"
git push origin main
# Netlify auto-deploys on push
```
