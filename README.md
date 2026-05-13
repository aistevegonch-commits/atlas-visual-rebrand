# Atlas Visual Rebrand

A complete rebrand from **Andrew's Production** to **Atlas Visual** — agency-grade identity, positioning, and pitch presentation for a scalable real estate video production company.

---

## Project Overview

Atlas Visual is built for scale. The rebrand moves away from a personal-name operation and establishes an independent agency identity capable of attracting investment firms, developers, and corporate accounts nationwide.

This repository contains the interactive brand presentation and supporting assets.

---

## File Structure

```
atlas-visual-rebrand/
├── index.html          # Primary website / interactive pitch deck (1920×1080)
├── video.html          # Video composition source (identical scenes, used for rendering)
└── README.md           # This file
```

- **index.html** — Open in any modern browser to view the full 7-scene animated presentation.
- **video.html** — Used as the source composition for the HyperFrames video render.

---

## Viewing Locally

No build step or server is required.

```bash
# macOS
open index.html

# Or with any static server
npx serve .
# Then visit http://localhost:3000/index.html
```

The presentation is optimized for a **1920×1080** viewport and uses Google Fonts (Space Grotesk, Inter) loaded via CDN.

---

## How the Video Was Rendered

The pitch video was produced using **HyperFrames**, a browser-to-video composition pipeline:

1. **Composition source**: `video.html` defines 7 timed scenes (`data-start` / `data-duration`) with GSAP-powered animations.
2. **Rendering**: HyperFrames captures each scene at 1920×1080, 60 fps, exporting a seamless video file.
3. **Delivery**: The final render is suitable for Telegram, LinkedIn, website hero backgrounds, and investor pitches.

> If you need to re-render, load `video.html` in HyperFrames (or any Puppeteer/Playwright-based screen recorder) and capture from `t=0` to `t=92` seconds.

---

## Deployment Recommendations

| Asset | Recommended Platform | Notes |
|---|---|---|
| **Website** | Vercel, Netlify, or GitHub Pages | Zero-config static hosting. Connect the repo for auto-deploy on push. |
| **Video** | Telegram, LinkedIn, or local file | The render is self-contained; no streaming host required for direct sharing. |
| **Custom domain** | Namecheap, Cloudflare Registrar | Secure `atlasvisual.com` or similar before public launch. |

### Quick Vercel Deploy
```bash
npm i -g vercel
vercel --prod
```

---

## Brand Assets Summary

### Color Palette
- **Deep Space**: `#06070a` — Primary background
- **Gold Accent**: `#d4a853` — CTAs, highlights, labels
- **Muted Text**: `#8b8f9a` — Secondary copy
- **Surface**: `#11131a` — Card and panel backgrounds

### Typography
- **Display**: Space Grotesk (700) — Headlines, pricing, data
- **Body**: Inter (300–700) — Paragraphs, labels, UI

### Positioning
- **Tagline**: *Local Now. Nationwide Next.*
- **Model**: Film. Cut. Deliver.
- **Target**: Investment firms, developers, corporate accounts
- **Pricing**: Three clear tiers ($1.2K–$18K) with project-based fees

---

## Next Steps

1. **Register domain** — Secure `atlasvisual.com` (or preferred variant) and set DNS.
2. **Form LLC** — Establish the legal entity under the Atlas Visual name.
3. **Deploy website** — Push `index.html` to Vercel/Netlify and point the custom domain.
4. **Social media setup** — Claim handles on Instagram, LinkedIn, and TikTok.
5. **Distribute video** — Share the HyperFrames render across Telegram, LinkedIn, and email outreach.
6. **Book first Signature-tier client** — Target 60 days to first $3.5K–$7.5K project.

---

*Atlas Visual • Rebrand Blueprint • 2026*
