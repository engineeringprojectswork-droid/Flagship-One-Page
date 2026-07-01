# Brief — design a PHONE-ONLY version of the Medmac Flagship Story

**From:** Claude Code (I own the routing/hosting/backend side)
**To:** Claude Design (you own the phone experience)
**Repo:** `engineeringprojectswork-droid/Flagship-One-Page` — you have full access to these files.

---

## The short version

There is already a finished **desktop** version I love and am keeping unchanged. I want a **brand-new, separate experience built specifically for phones**, living at its own URL. Phone visitors get auto-routed to it; PC visitors keep the current design. Build the phone experience with **full creative freedom** — the only constraints are a few small technical hooks (below) so your output plugs cleanly into the routing and static hosting I'm building.

**Do not touch the desktop version.** It stays as the PC experience.

---

## What already exists (your source of truth)

- **`Medmac-Flagship-Redesign.dc.html`** — the editable Design Component source for the desktop story. This is where all the real copy, numbers, EN/AR text, honest-framing lines, and scene structure live. **Read numbers and text verbatim from here.**
- **`index.html`** — the compiled desktop page (a self-contained bundle). This will be renamed/served as the desktop URL; leave it alone.
- **`uploads/assets-pack/NUMBERS.md`** — the single source of truth for every figure. If a number isn't here with a source, it does not go on screen.
- **`public/media/…`** and **`uploads/assets-pack/…`** — the real screenshots/media already in the repo. Reuse these.
- **`support.js`** — the desktop render runtime (for reference only).

---

## What I want

A **phone-first reimagining of the same 9-system story** — not the desktop layout squeezed down, but its own native mobile experience: designed thumb-up, portrait-first, for how people actually hold and swipe a phone. Vertical storytelling, full-bleed scenes, snap/scroll choreography, gesture-driven reveals, tactile motion — your call.

### Creative freedom — go big
**Do NOT hold back on graphics, animation, or ambition to "save performance."** Heavy motion, WebGL/canvas, particle/gradient work, scroll-linked choreography, rich transitions — all welcome and encouraged. Treat the phone as a first-class canvas, not a constraint.

The **only** ask: it must still **boot and stay navigable on a normal modern phone**. Progressive / lazy loading as scenes enter view is encouraged — but that's a *technique to enable richness*, not a cap on it. Don't sacrifice the vision.

---

## Content — same story, same real data (hard rule)

- Cover the same beats as desktop: intro/hero, the thesis, the **9 systems** (01 Paid social, 02 Audience growth / al-Maali, 03 CRM / Marketing ops, 04 Brand & content, 05 Software / sheep app, 06 Hiring automation, 07 Web · live, 08 AI operating model, 09 Career OS), and the contact finale.
- **REAL DATA ONLY.** Every number must trace to a source. Pull the verbatim numbers, the EN + Arabic copy, and the honest-framing lines directly from `Medmac-Flagship-Redesign.dc.html` and `uploads/assets-pack/NUMBERS.md`. Do not invent, re-round, or add any figure not sourced there.
- Keep al-Maali's verified endpoints (**FB 9.2K→1M+, IG 3K→50K, YT 0→43K, TikTok 0→33K**) and the real per-post metrics. **Do NOT add an invented follower growth curve** — there is no time-series in the source data.
- Keep CRM/HR screenshots **redacted** (they already are).
- Keep it **fully bilingual EN/AR** with a working language toggle and correct **RTL** handling (desktop uses a `lang` prop + `[dir]`).
- **Contact finale must use these real links** (already live on desktop):
  - WhatsApp → `https://wa.me/96590022918`
  - Email → `mailto:medo433447@gmail.com`
  - LinkedIn → `https://www.linkedin.com/in/mohamed-mahmoud-5a748b243`

---

## Technical hooks I need (small — they don't constrain the design)

1. **Static hosting, no server.** It will be served as a static file on GitHub Pages at its own path (`/mobile.html`). It must run by just opening the file — no server-side code, no build step required at view time.
2. **Deliverable format.** Prefer a **single self-contained `.html`** (assets inlined, like the desktop `index.html`). If that's impractical, deliver the raw source **plus a plain list of every external asset file and the exact repo path each should live at** — I'll commit them.
3. **Asset paths.** Anything referenced by path must use **root-relative paths** that resolve from the site root (e.g. `public/media/…`), same convention as desktop — or be inlined. No paths that assume a subfolder.
4. **"View desktop" control.** Include a clearly-marked link/button with a **stable hook** I can target — e.g. `<a data-view="desktop">Desktop</a>`. You can point it at `/desktop.html`, or leave the href empty and I'll wire it. (Note for you: there is **no remembered preference** — tapping it just takes the user to the desktop URL for that visit.)
5. **Viewport + safe areas.** Use `<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">`. **No horizontal scrolling.** Respect notches / home indicator via `env(safe-area-inset-*)`.
6. **Touch-first.** No hover-only interactions. Works in **portrait and landscape**.
7. **External deps are fine — just list them.** The desktop pulls React, `@babel/standalone`, and Google Fonts from unpkg/Google at runtime. If your build uses any CDN, **tell me the full list of external URLs** so I can confirm they're reachable from the host (and know the page needs a network connection).

---

## Deliverable checklist

- [ ] The phone `.html` (self-contained if possible).
- [ ] A short note listing: (a) any external **asset files** and their intended repo paths, and (b) any **CDN URLs** used.
- [ ] Confirmation it renders standalone (opens by double-click) with no horizontal scroll on a phone viewport.

I'll handle everything else: device detection, the redirect router, wiring the desktop/mobile toggle, committing assets, and deploying.

---

## Appendix — how it gets served (the environment you're targeting)

The site is on **GitHub Pages (static, `.nojekyll`)**. There is no server, so device detection is a tiny **client-side router**:

```
/               → router page. Sniffs phone vs. desktop (user-agent +
                  matchMedia/touch + width) and location.replace()s to the
                  right full page. Always auto-detects on each visit —
                  no stored preference.
/desktop.html   → the current desktop bundle (unchanged). Shareable. Never redirects.
/mobile.html    → YOUR new phone experience. Shareable. Never redirects.
```

So: a phone hitting the main link lands on your page automatically; a PC lands on the desktop one. Both full pages have their own clean, directly-shareable URLs, and neither redirects once you're on it — only `/` routes. Your "View desktop" hook simply points a mobile user at `/desktop.html` for that session.

That's the whole integration surface. Everything else is yours — go make it great. 🚀
