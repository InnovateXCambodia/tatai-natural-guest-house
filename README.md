# Tatai Natural Guest House Website

## Locked baseline
This repository package is based on the approved **v18** website master.

The visible website in `index.html` is preserved from the locked v18 baseline.

## Current structure
- `index.html` — approved website master
- `assets/brand/` — approved light and reverse logo source files
- `404.html` — custom 404 page
- `thank-you.html` — reserved for the future inquiry form flow
- `robots.txt` — currently blocks indexing during staging
- `netlify.toml` — Netlify publish and basic security headers
- `.gitignore` — repo cleanup rules

## Deployment workflow
GitHub `main` → Netlify staging → QA → domain cutover → production indexing

## Before production indexing
When the real domain is confirmed and the site passes QA:
1. Change `robots.txt` from `Disallow: /` to `Allow: /`.
2. Add the production `sitemap.xml` using the confirmed live domain.
3. Add/verify canonical URLs and production-domain metadata if needed.
4. Submit the sitemap in Google Search Console.

## Important
The current approved website uses direct Email and Telegram booking/contact CTAs.
A Netlify inquiry form is **not yet present in the locked v18 page** and should only be added as a deliberate future revision, not silently during packaging.
