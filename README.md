# Jissen-Ryu Martial Arts

The website for Jissen-Ryu Martial Arts — Mandeville, Louisiana.

> 進化 · 伝統 — *Shinka · Dentō* — Evolving Tradition

## Live site

When GitHub Pages is enabled (instructions below), this site is published at:

**https://chadhowell11.github.io/Jissen-Ryu/**

## What's in here

```
/
├── index.html          The site — a single, self-contained HTML page
├── assets/
│   ├── logo.png        Web-optimized logo (512px) used in the page
│   ├── logo-hires.png  Original high-resolution logo, archived
│   └── favicon.png     Browser tab icon
├── .nojekyll           Tells GitHub Pages to serve files as-is (no Jekyll processing)
└── README.md           This file
```

## Viewing locally

No build step — just open `index.html` in a browser. If you want a proper local server (recommended for testing on mobile devices on the same network):

```bash
# Python 3
python3 -m http.server 8000

# Or with Node
npx serve .
```

Then open `http://localhost:8000`.

## Enabling GitHub Pages

After the first push:

1. Go to **Settings → Pages** in this repo
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main` · Folder: `/ (root)`
4. Save

The site goes live at `https://chadhowell11.github.io/Jissen-Ryu/` within a minute or two. Every push to `main` redeploys automatically.

## Editing content

All content lives directly in `index.html`. A few useful entry points:

| Looking for | Find it near |
|---|---|
| Colors, fonts | The `:root { ... }` block at the top of the `<style>` |
| Phone, address, hours | The `<section class="s contact">` near the bottom |
| Programs | The `<section class="s programs">` block |
| Schedule grid | The `<section class="s schedule">` block |
| Instructor cards | The `<section class="s instr">` block |
| Trial offer | The `<section class="cta-band">` block |
| Footer links | The `<footer>` at the very bottom |

Colors are set via CSS custom properties — change them once in `:root` and they update everywhere:

```css
--paper:      #f3ece0;   /* warm cream background */
--ink:        #15110d;   /* deep ink text */
--crimson:    #b22724;   /* primary accent (logo red) */
--indigo:     #1d3a7c;   /* secondary accent (logo blue) */
```

## Roadmap (rebuild project)

This single-page version is the **kickoff** for the full rebuild. Likely next moves:

- [ ] Pull real content from the current Mandevillekarate.com site
- [ ] Real instructor photos and bios
- [ ] Real phone, address, hours, pricing
- [ ] Split into multi-page structure (Home / Programs / About / Schedule / Contact)
- [ ] Contact form with email delivery
- [ ] Calendar integration for events and seminars
- [ ] Custom domain (CNAME) — point e.g. `mandevillekarate.com` at GitHub Pages

## License

© Jissen-Ryu Martial Arts. All rights reserved.
