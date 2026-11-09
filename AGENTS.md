# Repository agent instructions

This repository is the Astro + TypeScript website for tanzyyy-dev.

## Required design guidance

**Before any screen/UI change**, read `.agents/skills/portal-design/SKILL.md` and follow its workflow and design constraints. This includes changes to layouts, components, CSS, navigation, responsive behavior, visual assets, and user-facing page structure. Do not begin implementing UI changes before reviewing that file.

For non-UI changes, use the relevant repository conventions; consult the design skill if the change affects the rendered experience.

## Working rules

- Keep Japanese as the default site at `/` and English at `/en/`. Maintain parity when editing user-facing content or navigation.
- Use Astro + TypeScript and static output compatible with GitHub Pages.
- Do not invent project screenshots, demo URLs, product claims, or additional projects. Project information is manually maintained in `src/data/content.ts`.
- Make focused changes. Do not alter GitHub Pages settings, GitHub Actions triggers, or deployment configuration unless explicitly requested.
- Before declaring work complete, run `npm run build` when dependencies are available, and report what was and was not verified.
