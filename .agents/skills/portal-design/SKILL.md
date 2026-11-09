---
name: portal-design
description: Design and review the tanzyyy-dev Astro project portal UI. Read before modifying layouts, components, styles, navigation, responsive presentation, or other user-facing screens.
---

# Portal design skill

## Purpose

Build a distinctive, useful **software and project directory for ordinary visitors**, not a generic developer portfolio or an experimental design showcase. Help visitors quickly understand what each project does, see what it looks like, and find its detail page, demo (when available), or source.

## Product context

- Site: `tanzyyy-dev.github.io`; Astro + TypeScript, static GitHub Pages.
- Japanese is the default (`/`); English lives under `/en/`.
- Categories: Games, Services, Contents, Skills.
- Initially there is only one project. Do not fabricate volume, popularity, ratings, search demand, or rankings.
- Project descriptions and links are manually maintained; unavailable demo links must not appear functional.
- The pixel-art schnauzer is an identity asset, **not a mandate to use mint green as the site's palette**.

## Design direction

- **Information architecture:** Take inspiration from familiar software directories such as 窓の杜: clear titles, categories, summaries, concrete actions, and predictable navigation. This is a structural reference, not an instruction to copy its visual styling.
- **Project presentation:** Learn from Playdate's game catalog in giving individual works a recognizable visual identity and room for genuine screenshots or artwork, without imitating its layout.
- Make the project itself the focal point. Use authentic imagery when available; otherwise choose a clearly intentional placeholder and do not misrepresent it as a screenshot.
- Favor legible hierarchy, precise spacing, useful metadata, and clear link affordances over decorative effects.
- Avoid recognizable generic AI-site tropes: arbitrary mint/green palettes, white-on-pastel rounded-card grids, excessive pill badges, ornamental gradients, empty hero slogans, and repetitive cards without a content purpose.
- Do not assume a color palette, typography, or visual motif has been approved. Propose choices based on the site's content and obtain agreement before large visual changes.

## Responsive layout principles

- No oversized generic hero, filler slogan, or repeated introduction. The home page should immediately show the actual project.
- On desktop, use a compact two-column project feature: visual on the left, title, summary, and primary action on the right.
- On mobile, use one column ordered visual → title → summary → primary action; preserve natural vertical scrolling rather than forcing viewport height.
- Keep page spacing proportional to content, and avoid decorative empty sections. Do not show filters when there is only one project.
- Prefer a simple visible navigation over a hidden hamburger for just a few destinations. Touch targets should be comfortable (around 44px).

## Workflow for screen changes

1. **Inspect before designing.** Read the relevant Astro pages, shared components, `src/styles/global.css`, and content model. Check current screenshots or a local preview when possible. State what is observed versus inferred.
2. **Identify the visitor task and problem.** Explain what is confusing or visually weak and why a proposed change improves discovery, comprehension, or action.
3. **For substantial redesigns, present distinct options first.** Compare 2–3 concrete directions with trade-offs and wait for selection before implementing. Do not silently choose a new visual system.
4. **Implement the selected direction** with reusable components and minimal unnecessary complexity. Preserve existing routes and content unless changes are approved.
5. **Verify.** Check mobile and desktop layouts, keyboard focus, contrast, accessible names, image alt text, broken links, and both language routes. Run `npm run build` when possible; disclose any unverified items.

For small, explicit changes (for example a favicon or a typo), implement directly without inventing a redesign exercise.

## UI quality checklist

- A first-time visitor can tell what the site offers and where to click.
- Project title, category, short description, and available actions are easy to scan.
- One project does not look like an empty marketplace; filters and empty states are purposeful.
- Layout works at narrow mobile widths without horizontal scrolling.
- Focus indicators are visible, semantics are correct, and navigation works without a mouse.
- Japanese and English layouts both accommodate text length.
- SEO/OGP metadata and actual project links remain accurate.
- No fabricated screenshots, testimonials, metrics, demos, or project entries.

## Repository pointers

- `src/layouts/Base.astro`: shared document structure and navigation.
- `src/components/`: project list and detail presentation.
- `src/styles/global.css`: global styling.
- `src/data/content.ts`: project data and Japanese/English copy.
- `src/pages/`: localized routes.
