# ajaygoldsmith-portfolio

My personal corner of the internet. Built from scratch using plain HTML, CSS, and JavaScript — no frameworks, no build tools, just code and a lot of trial and error.

Live at **[ajaygoldsmith.me](https://ajaygoldsmith.me)**

---

## Why I built this

I wanted a place that actually feels like me — not a template, not a cookie-cutter developer portfolio. Something that shows I can build and deploy things, holds my projects, and also has space for my shayris because that's a real part of who I am.

Started this in my first year of B.Tech ECE at GGV Bilaspur. Figured the best way to learn frontend seriously was to build something I actually cared about.

---

## What's inside

The site is a single HTML file. Everything — styles, scripts, layout — lives in `index.html`.

**Sections:**
- **Hero** — quick intro, what I do, two CTA buttons
- **About** — background, a stat card, a shayri, and a nature card (because sitting outside genuinely helps me think)
- **Skills & Stack** — tech I use, broken into a grid of tools, a Frontend card, Deploy card, ECE fundamentals, and soft skills
- **Projects** — six projects with tags and links. Featured one gets a wide card
- **Leadership** — roles I've held at GGV and what I've learned from them
- **Poetry & Shayri** — three short poems and one long featured piece, all original
- **Contact** — social links and a working contact form

---

## Tech used

| What | Why |
|------|-----|
| HTML / CSS / JS | Everything. No React, no Tailwind, no bundler |
| Instrument Serif | Headings — elegant and a little literary |
| DM Sans | Body text — clean, readable |
| Noto Serif Devanagari | Hindi/Urdu poetry |
| EmailJS | Contact form — messages go straight to my Gmail |
| Cloudflare Turnstile | Spam protection on the contact form |
| Cloudflare Pages | Hosting + CDN + email obfuscation |

---

## Features worth mentioning

**Glow cards** — the bento grid cards have a rainbow conic-gradient border that follows your mouse cursor and glows on hover. Built with `@property --glow-angle` and a CSS keyframe animation. No JS needed for the effect itself.

**Bento grid layout** — 12-column CSS Grid. Cards span different columns to create an asymmetric, editorial look. Collapses gracefully on mobile.

**Mobile navigation** — on smaller screens the nav links are hidden and a hamburger button opens a slide-in drawer from the right side. Overlay behind it closes it on tap.

**Scroll animations** — cards fade up as they enter the viewport using IntersectionObserver. No library needed.

**Contact form** — integrated with EmailJS. Validates name, email format, and message before sending. Turnstile verification blocks bots. Clears fields and resets on success.

**Ticker** — scrolling text strip between hero and about section. Pure CSS animation.

---

## Running locally

No setup needed. Just clone and open.

```bash
git clone https://github.com/TrulyAjay/portfolio
cd portfolio
# open index.html in your browser
```

Or just drag `index.html` into any browser window.

> Note: The contact form won't work locally since EmailJS and Cloudflare Turnstile only run on the live domain. Everything else works fine offline.

---

## Project structure

```
portfolio/
└── index.html       # The whole site
└── README.md        # You're reading this
```

That's genuinely it. One file.

---

## Deployment

Hosted on **Cloudflare Pages**.

1. Push to GitHub
2. Connect repo to Cloudflare Pages
3. Build command: *(none — it's static)*
4. Output directory: `/` or leave blank

Cloudflare handles the CDN, HTTPS, and email obfuscation automatically.

---

## Things I learned building this

- How `@property` works in CSS for animating custom properties
- Intersection Observer API for scroll-triggered animations
- How to structure a proper mobile-first responsive layout without a framework
- EmailJS integration and basic form validation
- Cloudflare Pages deployment and how their email obfuscation works
- Why `rel="noopener noreferrer"` matters on external links
- That a single HTML file can do a lot more than people give it credit for

---

## What's next

- Add a photo to the hero section
- Update project links as more things get built and deployed
- Maybe a dark mode toggle someday
- Keep adding poems as I write them

---

## Contact

If you want to reach me — the contact form on the site works, or:

- **Email:** [imdajayg@gmail.com](mailto:imdajayg@gmail.com)
- **GitHub:** [@TrulyAjay](https://github.com/TrulyAjay)
- **LinkedIn:** [Ajay Kumar](https://www.linkedin.com/in/ajay-kumar-73b63139b)
- **Instagram:** [@imd_ajay](https://instagram.com/imd_ajay)

---

*B.Tech ECE · Guru Ghasidas Vishwavidyalaya, Bilaspur · 2025–2029*
