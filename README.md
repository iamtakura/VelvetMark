# Velvetmark Agency Website

Velvetmark is a premium, high-aesthetic single-page agency website built in Astro and Vanilla CSS. It features custom GSAP ScrollTrigger animations, a responsive modern design, interactive services, a visual process timeline, and structured pricing models.

Live URL: **[https://iamtakura.github.io/VelvetMark/](https://iamtakura.github.io/VelvetMark/)**

---

## ✨ Features & Architecture

- **Premium Branding & Typography:** Uses Google Fonts with *Bebas Neue* for high-impact editorial headings and *Outfit* for crisp body text.
- **Micro-Animations & Smooth Experience:**
  - Dynamic **Custom Cursor** (crimson dot) with GSAP lag-follow that expands and scales when hovering over interactive components.
  - Page scroll-progress bar at the top of the viewport.
  - Transparent fixed header that dynamically shifts background opacity and blurs using `backdrop-filter` on scroll.
- **Word-by-Word Animation:** Headline text uses GSAP ScrollTrigger to split and stagger entrance word-by-word.
- **Interactive Sections:**
  - **Hero:** Full `100vh` introduction with an animated accent underline.
  - **Work:** Alternating row showcases featuring real project screenshots.
  - **Services:** Clean 3-column top-bordered cards that scale and hover.
  - **Process:** Step-by-step methodology timeline with desktop connecting lines and sequence staggers.
  - **Pricing:** 4-column responsive grid with a highlighted recommended tier and pre-filled WhatsApp interest links.
  - **Contact:** Clean call-to-action layout triggering pre-filled WhatsApp conversations.

---

## 🛠️ Technology Stack

- **Framework:** [Astro v6](https://astro.build/) (Static Mode)
- **Styling:** Vanilla CSS variables for a central design system
- **Animation:** GSAP (GreenSock Animation Platform) + ScrollTrigger

---

## ⚙️ Development & Build Commands

All commands are run from the root of the project:

```bash
# Install dependencies
npm install

# Start local dev server at localhost:4321
npm run dev

# Build the production site (compiles to ./dist/)
npm run build

# Preview your production build locally
npm run preview
```

---

## 🚀 GitHub Pages Deployment

The site is configured to build and deploy to GitHub Pages automatically via GitHub Actions:

1. **Astro Base Path:** Configured in `astro.config.mjs` with `site` set to `https://iamtakura.github.io` and `base` set to `/VelvetMark` to correctly map relative asset routes.
2. **GitHub Actions Workflow:** `.github/workflows/deploy.yml` triggers on any push to the `master` or `main` branches. It handles dependency installation, production compilation, and uploads the built `dist/` directory to GitHub Pages.
