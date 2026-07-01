# Phone experience — delivery note

**Deliverable:** `mobile.html` — a single self-contained file (~7.8 MB). Serve it at **`/mobile.html`**.
**Editable source:** `Medmac Flagship - Mobile.dc.html` (recompile with the same inliner to regenerate `mobile.html`).

Built to the brief: a phone-first reimagining of the same 9-system story — vertical, scroll-scrubbed, full-bleed cinematic scenes with meaningful per-system explainer animations. **Not** the desktop squeezed down. Desktop is untouched.

---

## (a) External asset files to commit
**None.** Every screenshot / image is inlined into `mobile.html` (base64 → blob at boot), same self-containment level as the desktop `index.html`. Nothing else to commit for it to render.

*(The editable `.dc.html` source references the real media at root-relative `public/media/…` paths — the same ones already in the repo — so it renders in-repo too. The compiled `mobile.html` needs none of them.)*

## (b) CDN URLs used (page needs a network connection)
Same external surface as the desktop bundle, minus Babel:
- `https://unpkg.com/react@18.3.1/umd/react.production.min.js`
- `https://unpkg.com/react-dom@18.3.1/umd/react-dom.production.min.js`
- `https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=IBM+Plex+Sans+Arabic:wght@400;500;600;700&display=swap`
- `https://fonts.gstatic.com/…` (woff2 files the above stylesheet pulls)

No `@babel/standalone` (logic is plain JS, not in-browser JSX).

---

## Technical hooks (all implemented)
- **Viewport:** `<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">`.
- **No horizontal scroll** (verified at 390×844); `overflow-x: clip` on body.
- **Safe areas:** top/bottom chrome and every scene pad with `env(safe-area-inset-*)`.
- **Touch-first:** no hover-only interactions; works portrait and landscape.
- **"View desktop" control:** `<a data-view="desktop" href="/desktop.html">` — top-right in the header **and** in the contact finale. Repoint the href or wire it as you like; the hook is stable.
- **Bilingual EN/AR:** auto-detects `navigator.language` on load (Arabic → `ar`, else `en`), with an always-present **EN / ع** toggle that sets `dir="rtl"` and swaps every string. No stored preference.

## Real data only
Every number and line is verbatim from `Medmac-Flagship-Redesign.dc.html` + `uploads/assets-pack/NUMBERS.md`. al-Maali **animates the climb only between the two verified endpoints** (9.2K → 1M+) — no invented in-between follower series; the four endpoints (FB 9.2K→1M+, IG 3K→50K, YT 0→43K, TikTok 0→33K) and real per-post metrics are shown as-is. CRM/HR screenshots stay redacted. Contact finale: WhatsApp `wa.me/96590022918`, `mailto:medo433447@gmail.com`, LinkedIn `in/mohamed-mahmoud-5a748b243`.

## Confirmed
Opens standalone (double-click), renders, sticky scroll-scrubbing works, no horizontal scroll on a phone viewport. Chapters: Intro → thesis → 01–09 → Contact.
