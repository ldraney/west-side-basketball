# Westside Kings & Queens — Project Instructions

## Tech Stack

- **Static site**: Plain HTML/CSS/JS — no build step, no frameworks, no bundlers
- **Hosting**: GitHub Pages (source: main branch, root folder)
- **Payments**: Stripe Payment Links (no backend)
- **Fonts**: System fonts only — no external CDN requests

## File Structure

```
west-side-basketball/
├── index.html           # Landing/tryouts page
├── coaches.html         # Coach bios
├── success.html         # Post-payment redirect
├── css/style.css        # Shared responsive styles
├── js/main.js           # Mobile nav, smooth scroll
├── assets/images/       # Logos, photos, favicon, OG image
```

## Conventions

- **Mobile-first CSS** — base styles for mobile, `min-width` media queries for larger screens
- **CSS custom properties** for all design tokens (colors, spacing, typography)
- **Relative paths** for all internal links (site lives at `/west-side-basketball/` subdirectory)
- **System font stack**: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif`
- **Dark sports aesthetic**: Navy/charcoal backgrounds + orange/gold accents
- **Semantic HTML**: Use proper heading hierarchy, landmarks, and ARIA where needed
- **Progressive enhancement**: Core content works without JS

## Branch Workflow

- All work on feature branches: `{issue-number}-{short-description}`
- All changes via pull requests to main
- Never push directly to main after bootstrap

## Key Decisions

- Stripe Payment Links (not Checkout Sessions) — no backend needed
- `.nojekyll` file required to prevent GitHub Pages Jekyll processing
- No external dependencies — everything is self-contained
