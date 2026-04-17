# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev       # Start dev server at localhost:4321
npm run build     # Build production site to ./dist/
npm run preview   # Preview production build locally
```

No test or lint commands are configured yet.

## Architecture

This is an **Astro v6** static site that generates landing pages from user-provided product descriptions using AI. Users fill out a form (product name, description, target audience, key benefits, tone of voice) and receive a complete landing page they can copy or download as HTML.

**Source layout:**
```
src/
├── layouts/Layout.astro   # Root HTML shell; imports global CSS, sets page title
├── pages/index.astro      # Single page: two-panel layout (form + preview)
└── styles/global.css      # Design tokens, typography scale, CSS reset
```

**Design system** lives entirely in `global.css` as CSS custom properties:
- Primary: indigo palette (`--color-primary-*`)
- Accent: rose palette (`--color-accent-*`)
- Neutral: gray palette (`--color-gray-*`)
- Typography scale: `heading-one` through `heading-four`, `font-small`, `font-xsmall`

**Layout:** Mobile-first single column; at 768px, switches to a 2-column grid (form panel `1fr`, preview panel `50%`).

**AI integration** — the form submission logic, API calls, and HTML copy/download functionality are not yet implemented. The preview panel currently contains an iframe placeholder.
