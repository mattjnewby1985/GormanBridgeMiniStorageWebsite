# Gorman Bridge Mini Storage Website

Static one-page site for https://www.gormanministorage.com, hosted on GitHub Pages (`CNAME`).

- `index.html` contains all markup, CSS and icons inline. It has no build step and no dependencies.
- Rentals, pricing and payments are handled by ccStorage: https://gormancentralgroup.ccstorage.com/find_units
- `images/`: optimized logo (`logo-240.webp`, `logo-480.webp`), social share image (`og-image.jpg`), and the original logo source PNGs.
- `favicon.png`, `apple-touch-icon.png`, `robots.txt`, `sitemap.xml`, `404.html`.

To edit: change `index.html`, commit, and push to `main`. GitHub Pages republishes automatically.
Keep the business details (phone, hours, address) in sync between the visible text and the JSON-LD block in `<head>`.
