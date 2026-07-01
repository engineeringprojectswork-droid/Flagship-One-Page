# Flagship One-Page

A one-page, scroll-driven site — **"A whole marketing team. In one person."** — covering 9 real systems Mohamed runs for Medmac Kuwait (paid social, audience growth, CRM, brand, software, hiring automation, live website, AI operating model, career OS). Bilingual EN/AR.

## Live site

`index.html` at the repo root is the finished site as a single self-contained file (images, fonts, and the render runtime are inlined — no build step, no server). GitHub Pages serves it directly as the site root.

**To enable GitHub Pages** (one-time, in repo Settings → Pages): set Source to "Deploy from a branch", pick this branch, folder `/ (root)`. The site will then be live at `https://engineeringprojectswork-droid.github.io/flagship-one-page/`.

## Repo contents

- **`index.html`** — the deployable site (self-contained, ~8MB due to inlined images).
- **`deploy/DEPLOY-for-Claude-Code.md`** — deploy notes, incl. two pre-launch items (placeholder contact links, optional live-capture scenes).
- **`Medmac-Flagship-Redesign.dc.html`**, **`Al-Maali - 4 Directions.dc.html`** — editable Design Component sources; re-export to regenerate `index.html`. Don't hand-edit `index.html` structurally.
- **`public/`** — supporting films and media referenced by the design sources.
- **`uploads/assets-pack/`** — sourced screenshots and verbatim numbers (`NUMBERS.md` is the single source of truth for every figure on screen).
- **`ASSET-REQUEST-for-Claude-Code.md`** — asset-gathering brief for the 9-project story redesign.
- **`support.js`** — render runtime used by the design sources.

## Before it goes fully public

1. **Contact links are placeholders.** The "Hire one. Get a team." section has WhatsApp/Email/LinkedIn chips reading `↗ add link` — replace with Mohamed's real links (WhatsApp: **90022918**; email + LinkedIn still needed).
2. Optional: capture live screenshots for the Web and AI-operating-model scenes (see `deploy/DEPLOY-for-Claude-Code.md`). Neither blocks launch.
