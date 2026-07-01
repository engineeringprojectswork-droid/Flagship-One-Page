# Deploy — Medmac Flagship Story

A one-page, scroll-driven site: **"A whole marketing team. In one person."** — 9 real systems Mohamed runs for Medmac Kuwait (paid social, audience growth, CRM, brand, software, hiring automation, live website, AI operating model, career OS). Bilingual EN/AR (a language toggle is wired via the `lang` prop).

**Governing rule: real data only.** Every number on screen traces to a source. If a figure isn't in `NUMBERS.md` (in the asset pack) with a source, it does not go on screen. Please preserve this when editing.

---

## What's in this zip
- **`Medmac-Flagship-Story.html`** — the finished site as a **single self-contained file**. All images, fonts, and the render runtime are inlined. It works offline — double-click to open, no build step, no server.
- **`DEPLOY-for-Claude-Code.md`** — this file.

---

## Fastest way to publish (no code)
Drag `Medmac-Flagship-Story.html` onto any static host:
- **Netlify Drop** (drag-and-drop, instant), **Vercel**, **Cloudflare Pages**, or **GitHub Pages**.
- Rename to `index.html` if the host serves a directory root.

That's the whole deploy. It's a static file.

## Cleaner: fold it into the existing Medmac site
The company site is already on Vercel (`medmac-kuwait.vercel.app`, Astro + TS + Tailwind). To ship this under the same domain/CI:
1. Drop `Medmac-Flagship-Story.html` into the Astro repo's **`public/`** as `public/story.html`.
2. It will serve verbatim at **`/story.html`** (Astro copies `public/` as-is — no processing). Optionally add a redirect/route `/story` → `/story.html`.
3. Commit → Vercel auto-deploys. Done.

> The file is ~7.9 MB because images are inlined (self-contained). If you prefer smaller/CDN-cached assets, the un-inlined source is a Design Component (`.dc.html`) authored in the design tool — ask Mohamed to export the raw source + `public/media/` folder instead, and reference the images normally. For a single-page brochure this size is fine; don't over-optimize.

---

## Before it goes fully public — 2 things

1. **Contact links are placeholders.** The final "Hire one. Get a team." section has three chips — **WhatsApp / Email / LinkedIn** — each currently reading `↗ add link`. Replace with Mohamed's real links (the company WhatsApp is the public number **90022918**; get his email + LinkedIn). These live in the source Design Component's contact section; easiest is to have Mohamed drop them in the design tool and re-export, OR edit the chips directly in the HTML if you're comfortable (search for `add link`).

2. **Optional — fill the two remaining scenes with live captures** (both currently use the real *numbers*, so they're honest as-is; screenshots would just strengthen them):
   - **07 · Web:** section shows the real Lighthouse scores (Perf 96 / A11y 100 / BP 100 / SEO 100). A live screenshot of the site + a fresh Lighthouse run would add proof. (`_TO-CAPTURE` in the asset pack has the shot list.)
   - **08 · AI operating model:** a redacted screenshot of the ranked RFQ output (23 found · 4 recovered) is the only [NICE] asset still not captured.
   Neither blocks launch.

---

## Editing notes
- **Don't hand-edit `Medmac-Flagship-Story.html`** for anything structural — it's a compiled/inlined build artifact. The editable source is the Design Component (`Medmac-Flagship-Redesign.dc.html`) in the design tool; re-export to regenerate this file.
- Small text/link fixes (like the contact links) are safe to do directly in the HTML if that's faster for you — just search the readable text.
- **Integrity:** the al-Maali section uses verified endpoints (FB 9.2K→1M+, IG 3K→50K, YT 0→43K, TikTok 0→33K) and **real per-post metrics** from post insights (26.7K likes; single-post reach 14.2M / 6.2M / 1.8M). There is **no follower time-series** in the source data — do not add an invented growth curve. CRM/HR screenshots are real exports with all PII redacted; keep them redacted.

Questions on any number → `NUMBERS.md` in the asset pack is the single source of truth.
