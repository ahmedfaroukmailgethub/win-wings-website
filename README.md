# WIN WINGS — Website

Marketing website for **WIN WINGS**, an aviation (in‑flight) catering and logistics
operator serving airline and aviation partners worldwide. *Serving the World Above the Sky.*

WIN WINGS is part of the **WIN GROUP** family of companies.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero, certifications, stats, overview |
| About | `about.html` | Company profile, vision, values |
| Services | `services.html` | Catering services (in‑flight, VIP, charter, crew, buy‑on‑board, etc.) |
| Operations | `operations.html` | Facilities, high‑loaders, logistics, coverage |
| Why Us | `why-us.html` | Advantages, airline‑partner testimonials |
| Contact | `contact.html` | Contact details and enquiry |

## Tech

- Static, multi‑page site — **HTML + CSS + vanilla JavaScript**. No build step.
- Single shared stylesheet: `style.css` (cache‑busted via `?v=` query on each page).
- Fonts via Google Fonts; airline partner logos and certification badges as image assets.

## Run locally

It's a static site, so any static file server works. For example:

```bash
# Python 3
python -m http.server 3000

# or Node
npx http-server . -p 3000
```

Then open <http://localhost:3000/index.html>.

## Deploy

Any static host works (GitHub Pages, Netlify, Vercel, S3, etc.). For **GitHub Pages**,
enable Pages on the default branch and the site is served from `index.html`.

## Structure

```
.
├── index.html / about.html / services.html / operations.html / why-us.html / contact.html
├── style.css
├── Airlines Logos/      # airline partner logos (transparent PNGs)
└── *.png / *.jpg / *.svg # brand logos, certification badges, photography
```

---

© WIN WINGS. All rights reserved.
