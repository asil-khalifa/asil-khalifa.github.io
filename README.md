# asilkhalifa.com

Personal portfolio and résumé site — hand-written HTML, CSS and JS, no build step.
Served by GitHub Pages from the repo root at [asilkhalifa.com](https://asilkhalifa.com).

| File | Purpose |
| --- | --- |
| `index.html` | All page content (single page) |
| `styles.css` | Design tokens, layout, light/dark themes, print stylesheet |
| `script.js` | Theme toggle, scroll reveal, active-nav highlighting |
| `favicon.svg` | Favicon |
| `CNAME` | Custom domain for GitHub Pages |

## Local preview

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Notes

- **Résumé download** uses the browser's print dialog — the print stylesheet in
  `styles.css` reflows the page into a clean document. To offer a real file instead,
  drop `resume.pdf` in the repo root and point the button at it.
- Theme follows the OS by default; the toggle overrides it and persists in `localStorage`.
- Content lives directly in `index.html` — edit the section you want and push.
