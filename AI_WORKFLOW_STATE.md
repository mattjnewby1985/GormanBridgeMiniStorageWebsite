# Project State

## Objective
Replace the ccStorage redirect on www.gormanministorage.com with a real, indexable marketing site; ccStorage remains the system for pricing, rentals and payments.

## Current State
Live on GitHub Pages from `main` (PRs #1, #2 merged). Owner verified all links and map on the live site (2026-11-12). No open work.

## Confirmed
- Units: 5x10, 10x10, 10x20; 3 car/small-trailer parking spaces (e.g. 6x10 utility trailer)
- Gate: automatic, 7:00 AM – 8:00 PM, 7 days
- Security: multiple cameras with live alerts to management
- Pricing lives only on ccStorage, never on the site
- Contact: tap-to-call (828) 338-8956 and info@gormanministorage.com; no contact form

## Changes
- `index.html`: single page, inline CSS + SVG icons, no dependencies or build step. Meta/Open Graph tags, `SelfStorage` JSON-LD, Google Maps embed, directions, Google Business Profile link, sticky mobile Call/Rent bar
- Links: Rent `https://gormancentralgroup.ccstorage.com/find_units`; Pay My Bill `https://gormancentralgroup.ccstorage.com/payment-methods/new`
- Removed HTML5 UP template, jQuery, Font Awesome, placeholder images (~3.5 MB)
- Added facility photo (`images/facility-800.webp`, `facility-1400.webp`, EXIF stripped), WebP logo, favicon, apple-touch-icon, `images/og-image.jpg`, `robots.txt`, `sitemap.xml`, `404.html`
- `_config.yml` excludes this file and README from the published site

## Verification
- Playwright render at 1280px and iPhone 13: no console errors, no horizontal scroll; JSON-LD parses
- Owner confirmed all links and map on the live site

## Unresolved (optional)
- Google Search Console: verify domain, submit `/sitemap.xml`
- Google Business Profile: Website field = domain; hours = 7 AM–8 PM daily
- More photos: gate/keypad, parking spaces
- Better Pay My Bill target if ccStorage has a general tenant login/payment URL

## Constraints
- Phone/hours/address appear in both visible text and the JSON-LD in `index.html` `<head>`; change both together
- Do not remove `CNAME` (custom domain)
- Anything pushed to `main` deploys automatically

## Relevant Files
- `index.html`, `images/`, `README.md`, `CNAME`, `sitemap.xml`, `_config.yml`

## Next Step
Owner: set up Google Search Console and submit the sitemap (no code change).
