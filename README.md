# Learn to Achieve — Website

The public website for **Learn to Achieve**, a California civic-technology nonprofit building free, open-source data tools and education programs for under-resourced learners.

🌐 **Live at:** [learntoachieve.us](https://learntoachieve.us)

---

## What this is

A single-page static site. No build step, no framework, no JavaScript dependencies. Just `index.html` + `favicon.svg`. Hosted on Vercel (or any static host).

---

## Stack

- **HTML / CSS** — single self-contained file
- **Google Fonts** — Fraunces (display serif), DM Sans (body), JetBrains Mono (UI/code accents)
- **Hosting** — Vercel (free tier)
- **Domain** — registered at Cloudflare Registrar

---

## Local preview

No build step. Open the file directly:

```bash
open index.html
```

Or for live-reload while editing, use any static-file server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

---

## Deployment

The repo is connected to Vercel. Pushes to `main` auto-deploy.

To deploy manually via Vercel CLI:

```bash
npm i -g vercel
vercel --prod
```

Custom domain (`learntoachieve.us`) is managed in the Vercel project's **Settings → Domains** panel and points back to Cloudflare DNS.

---

## Editing copy

Almost all copy lives directly in `index.html`. Sections are clearly commented:

- `<!-- ===== STATUS BAR =====` — top live-now strip
- `<!-- ===== NAV =====` — top navigation
- `<!-- ===== HERO =====` — first-fold headline + fact card
- `<!-- ===== THREE PILLARS =====` — Healthcare / Workforce / Education program cards
- `<!-- ===== FEATURED =====` — HEE deep-dive section
- `<!-- ===== THESIS =====` — through-line / mission narrative
- `<!-- ===== ROOTS =====` — historical Achiever Mentorship section
- `<!-- ===== TEAM =====` — current team + founders/board
- `<!-- ===== INVOLVE =====` — partner / contribute / donate
- `<!-- ===== FOOTER =====` — boilerplate, EIN, mailing address

---

## To-do (post-launch)

- [ ] Wire actual PayPal donation URL into the donate card (currently `#`)
- [ ] Generate proper 1200×630 OG image at `/og-image.png` for link previews
- [ ] Confirm Joseph's surname and title; update Team section
- [ ] Once IRS reinstatement is approved, swap "California nonprofit" → "501(c)(3) nonprofit" sitewide

---

## Org details

**Learn to Achieve**
California Public Benefit Nonprofit Corporation
EIN: 82-3970859
CA Entity Number: C4084984
Founded: 2017, Del Norte County, CA

Contact: learntoachieves@gmail.com

---

## License

Site source: MIT License (forkable, modifiable).
Brand assets, copy, and logo: © Learn to Achieve, all rights reserved.
