# addalaf.com — landing page

Static landing page for **Addalaf**, served by GitHub Pages at the apex domain **addalaf.com**.
It is a single static `index.html` plus assets and self-hosted fonts. **No build step, no
framework, no analytics, no cookies, no forms, no third-party requests.**

The web app lives separately at **app.addalaf.com** (a different repo); this repo does not touch it.

## Contents
- `index.html` — the page (copy + layout from the founder's design export `addalaf-landing-v1.html`, 2026-11-06; reproduced verbatim).
- `assets/` — images: `logo-full-lit.png`, `nav-mic-lit.png`, `bg-app-body.svg` (fixed skyline), `icon-profile.svg`, `icon-edit.svg`, and Apple's official `app-store-badge.svg`.
- `fonts/` — self-hosted **Roboto** (Apache-2.0) and **Montserrat** (OFL) as variable woff2 (latin), with their licence files.
- `og-image.png` (1200×630 share image), `favicon.svg` / `favicon.png` / `apple-touch-icon.png`.
- `CNAME` — the custom domain (`addalaf.com`). `.nojekyll` — serve files as-is.

## App Store link — TODO
The App Store listing isn't approved yet. The App Store URL lives in **ONE place**: the
`APP_STORE_URL` constant in the inline config `<script>` at the bottom of `index.html`.
Both "Download on the App Store" badges link to `#` until you set it. That script is a
plain config constant — it makes no network request and sets no cookie.

## Hero logo
`assets/logo-full-lit.png` is the current hero logo (the app's neon wordmark). The founder
will supply a hero-specific version later — swap that one file and the hero + og-image update.

## Fonts / licences
Roboto and Montserrat are both free to self-host. Licences are in `fonts/`:
`Roboto-LICENSE-Apache-2.0.txt`, `Montserrat-OFL.txt`. (Note: Roboto is Apache-2.0, not OFL.)
