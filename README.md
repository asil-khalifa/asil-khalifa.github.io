# asilkhalifa.com

Personal portfolio and résumé site — hand-written HTML, CSS and JS, no build step.
Served by GitHub Pages from the repo root at [asilkhalifa.com](https://asilkhalifa.com).

| File | Purpose |
| --- | --- |
| `index.html` | All page content (single page) |
| `styles.css` | Design tokens, layout, light/dark themes, print stylesheet |
| `script.js` | Theme toggle, scroll reveal, active-nav highlighting |
| `favicon.svg` | Favicon |
| `portrait.jpg` | Hero portrait (also the og:image) |
| `Asil-Khalifa-Resume.pdf` | The downloadable résumé |
| `CNAME` | Custom domain for GitHub Pages |

## Local preview

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Notes

- **Résumé download** serves `Asil-Khalifa-Resume.pdf` from the repo root. To update it,
  replace that file — the link and filename stay the same.
- **Portrait**: `portrait.jpg` is a 640x640 crop of the full-resolution photo, which stays
  untracked; `.gitignore` records the ffmpeg command that regenerates it.
- The print stylesheet still applies to Ctrl+P, and hides the nav, buttons and photo.
- Theme follows the OS by default; the toggle overrides it and persists in `localStorage`.
- Content lives directly in `index.html` — edit the section you want and push.
