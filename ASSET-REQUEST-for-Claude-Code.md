# 📦 Asset & data request — 9-project story redesign

**From:** Claude Design (working on the new story experiences)
**To:** Claude Code (you have all of Mohamed's files + the repo — please gather these and return a ZIP)
**Why:** I'm rebuilding how each of the 9 project stories is presented (bigger creative swing, promoting the interactive films, fixing pacing/mobile/repetition). To keep the **"real data only"** rule, every new scene must use **true screenshots and verbatim numbers**. I've already read the repo (`projects.ts`, `profile.ts`, `public/films/*`, the design system), so I mostly need **real screenshots** and any **growth-timeline data that isn't in the repo yet**.

> Owner's notes I'm working from: keep the al-Maali climb counter; the current scene *visuals* are placeholders to replace; the brand-system project should stay **conceptual** (no need to gather content images); sheep-app / CRM / tracking assets exist on his machine; al-Maali has a **growth folder** I can animate.

---

## How to return it
A ZIP — `assets-pack.zip` — with **one folder per project slug**. Each folder contains:
- **Screenshots** — PNG, high-res / retina, cropped clean (no desktop clutter). Name them by what they show, e.g. `crm-leads-tab.png`.
- **`data.md`** — every number I should use, **verbatim**, each with its **source + date**, plus the **EN + Arabic copy** to reuse (paste from `profile.ts` / the work component) and the **honest-framing line**.
- A top-level **`NUMBERS.md`** that lists every figure → where it traces to (so nothing is invented or re-rounded).

**Priority order:** `al-maali` → `crm` → `sheep-app` → `meta-ads` → the rest.
Tags below: **[REQUIRED]** = I'm blocked without it · **[NICE]** = improves it · **[SKIP]** = don't gather, I'll handle it conceptually.

---

## Per project

### 1. al-maali — Audience Growth  *(PRIORITY 1 — I'm building this first)*
- **[REQUIRED]** The **growth folder**: per-platform follower counts **over time** (dates 2021→2025) — even a rough monthly/quarterly series per platform. This is what makes the climb a real, animated curve instead of a guess.
- **[REQUIRED]** Confirm the end numbers verbatim: **Facebook 9.2K → 1M**, **Instagram 3K → 50K**, **TikTok 0 → 33K**, **YouTube 0 → 43K**, timeframe **2021–2025**.
- **[REQUIRED]** The honest-framing line (verbatim EN + AR).
- **[NICE]** Channel logo, a couple of real channel/post screenshots (proof of the 1M).

### 2. crm — Marketing Ops  *(PRIORITY 2 — owner says the current table doesn't convey the idea)*
- **[REQUIRED]** Real screenshots of the **12-tab CRM**: the Leads tab, the Dashboard, the **Ad-spend → leads funnel**, the Engineer hand-off queue, the **Accountability / SLA** tab.
- **[REQUIRED]** The **exact tab names** (EN + AR) and the **status taxonomy + its colours** (new / offer sent / hot / → engineer …).
- **[REQUIRED]** Verbatim counts: **12 tabs, 45 active leads, 22 offers, 200+ contacts, 0 closed** (and the honest line about why 0 is correct).

### 3. sheep-app — Software  *(owner has this)*
- **[REQUIRED]** Desktop-app screenshots (Windows + macOS if possible) — main screen(s), bilingual UI.
- **[REQUIRED]** The **59/59 test run** output and a **CI build** screenshot; the data **schema** (diagram or table list).
- **[NICE]** App icon, stack confirmation (Python · SQLite · CI).

### 4. meta-ads — Paid Social
- **[REQUIRED]** Confirm verbatim: **$0.84 / WhatsApp lead, 206 leads, $0.50 best campaign, CPM $2.03, CTR 0.65%**, total spend, reach, impressions, **2026 pilot** window.
- **[NICE]** 1–2 real ad-creative screenshots, a Meta Ads Manager view, a click-to-WhatsApp screenshot.
- **[REQUIRED]** Label the existing `public/img/work/*.jpg` (ad5, cover3, eq1–4, hire1, scaffold): what each shows + is it real/usable.

### 5. hr-system — Automation
- **[REQUIRED]** Verbatim funnel: **142 → 100 → 8** (and what each stage means), **7 scripts, 3 scheduled jobs**, the daily-clock/schedule.
- **[NICE]** A screenshot of the dedupe/scoring output or a scheduled-job log.

### 6. medmac-website — Web · Live
- **[REQUIRED]** The **live URL**, a **Lighthouse 96–100** screenshot, and a screenshot of the live site (desktop + mobile).
- **[NICE]** Stack confirmation (Astro · Vercel).

### 7. ai-workflow — AI Operating Model
- **[REQUIRED]** The **names of the 3 AI tools**, verbatim **23 tenders / 4 recovered**, and a one-paragraph description of what the workflow does.
- **[NICE]** Any artifact (a recovered-tender screenshot, a workflow diagram).

### 8. brand-system — Brand & Content  *(owner: keep it conceptual)*
- **[SKIP]** Don't gather content images.
- **[REQUIRED]** Just confirm the counts verbatim (**~254 files, ~144 videos, bilingual**) + one line on what the "content engine" covered. I'll present it abstractly.

### 9. my-resume — Career OS  *(this very site)*
- **[REQUIRED]** Confirm the **3 tools · 1 workflow · 1 person** framing and the **names of the 3 tools**.
- **[SKIP]** No screenshots needed — it's about the system itself.

---

## Global (applies to all)
- **[REQUIRED]** For every project, paste the **verbatim EN + Arabic** headline / lead / honest-line I should reuse, so I never rewrite a number or a claim.
- **[NICE]** Logos (al-Maali, Medmac) as transparent PNG/SVG.
- **[NICE]** Confirm the two bundled fonts (`alraimedia` black/bold) are cleared for use inside the films.

**One rule above all:** if a number isn't in `NUMBERS.md` with a source, I won't put it on screen. Thanks 🙏
