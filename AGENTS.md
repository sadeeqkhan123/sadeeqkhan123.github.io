# Repository agent instructions

This repository is the Astro + TypeScript website for tanzyyy-dev.

## Required design guidance

**Before any screen/UI change**, read `.agents/skills/portal-design/SKILL.md` and follow its workflow and design constraints. This includes changes to layouts, components, CSS, navigation, responsive behavior, visual assets, and user-facing page structure. Do not begin implementing UI changes before reviewing that file.

For non-UI changes, use the relevant repository conventions; consult the design skill if the change affects the rendered experience.

## Git commits and deployment safety

- **Commit all files belonging to one logical task in a single commit.** Prepare and review the complete change set before pushing; do not create or push one commit per file.
- **Push once per completed task**, after validation where possible. Avoid rapid consecutive pushes to `main`: each push triggers the GitHub Pages deployment workflow, and overlapping deployments can fail with HTTP 400 (`in progress deployment`).
- If additional fixes are needed, verify the previous deployment has completed before pushing again when practical.
- If the available GitHub tooling only supports one-file-per-commit writes, **do not silently use that approach**. Use a multi-file commit mechanism, or explain the limitation and request approval before proceeding.
- Do not change deployment configuration merely to compensate for unnecessary fragmented commits.

## Working rules

- Keep Japanese as the default site at `/` and English at `/en/`. Maintain parity when editing user-facing content or navigation.
- Use Astro + TypeScript and static output compatible with GitHub Pages.
- Do not invent project screenshots, demo URLs, product claims, or additional projects. Project information is manually maintained in `src/data/content.ts`.
- Make focused changes. Do not alter GitHub Pages settings, GitHub Actions triggers, or deployment configuration unless explicitly requested.
- Before declaring work complete, run `npm run build` when dependencies are available, and report what was and was not verified.
