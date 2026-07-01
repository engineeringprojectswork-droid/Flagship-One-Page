# assets-pack — for the 9-project story redesign

**For:** Claude Design · **From:** Mohamed (via Cowork) · **Date:** 2026-07-01
Built to your `ASSET-REQUEST-for-Claude-Code.md`. **Real data only** — every number traces to a file in `NUMBERS.md`; every screenshot is a real render/capture with personal data redacted.

## How it's organized
- **`NUMBERS.md`** — every figure → its source (read this first; the one rule).
- **one folder per slug** — each has a **`data.md`** (verbatim EN+AR copy, the honest-framing line, numbers) and its screenshots.
- **`_TO-CAPTURE/CAPTURE-THESE.md`** — the handful of shots that can only come from a live app/login (see status below).
- **`_fonts/`** — the AlRaiMedia fonts, confirmed (global [NICE]).

## Status by project
| Slug | Data (`data.md`) | Screenshots |
|---|---|---|
| al-maali (P1) | ✅ endpoints + honest line · ⚠️ no follower time-series exists | ✅ 8 real top posts + 5 yearly ad summaries |
| crm (P2) | ✅ + 12 tab names + status/colours | ✅ **5 rendered, PII-redacted** (dashboard, leads, ads→leads, accountability, colour key) |
| sheep-app (P3) | ✅ facts + schema · **corrected to v4.1** (folder had old v2; 80/80 not 59/59) | ✅ **EN + AR of the real v4.1 app** (from CI run #18) · CI-tab shot optional |
| meta-ads (P4) | ✅ + **CTR 0.65% now sourced** | ✅ real Meta metrics panel + 3 creatives + img-work labels · ⏳ Ads Manager [NICE] |
| hr-system | ✅ funnel 142→100→8 | ✅ **4 rendered, PII-redacted** (master tracker, all candidates, colour key, scoring) |
| medmac-website | ✅ Lighthouse + stack + URL | ⏳ live site + Lighthouse → `_TO-CAPTURE` |
| ai-workflow | ✅ 3 tools + 23/4 + paragraph | ⏳ rfq-list [NICE] → `_TO-CAPTURE` |
| brand-system | ✅ counts (keep conceptual) | — [SKIP] by request |
| my-resume | ✅ 3·1·1 framing | — [SKIP] by request |

## Integrity notes (please honour)
- **CTR 0.65%** was NOT in the repo — it's now sourced to the CRM's `📊 إعلانات ميتا` sheet (self-logged from the Meta export). Safe to use. CPC $0.31, CPM $2.03, frequency 2.1 come from the same sheet.
- **al-maali has no follower-over-time data.** Animate between the verified endpoints (FB 9.2K→1M, IG 3K→50K, TikTok 0→33K, YT 0→43K). The yearly `ad-summary-*.jpg` are **reach/spend, not followers** — don't relabel them.
- **All CRM/HR screenshots are redacted in the data before rendering**, and a regex safety-net (wa.me / http / @ / 8+ digit runs) was asserted to leave **0** contact-data cells. No client or candidate name, phone, email, lead WhatsApp, price, or offer value appears.
- The CRM dashboard independently corroborates the honest line: **207 contacts, 22 offers, 0 sold.**

## Global confirms (from `ASSET-REQUEST` "Global")
- **The 3 AI tools:** Cowork (controller/memory/briefs) · Claude Design (look) · Claude Code (build·git·deploy). Framing: **3 tools · 1 workflow · 1 person**.
- **Fonts:** `AlRaiMedia Black` + `AlRaiMedia Bold` are in `_fonts/` — they're in Mohamed's own marketing-plan kit, so cleared for use in the films.
- **Logos:** no standalone Medmac/al-Maali logo file exists in the project; the Medmac mark is embedded in the ad creatives (see `meta-ads/img-work-labels.md` → `cover3.jpg`). Capture a clean logo if a vector is needed.

## What's left
See `_TO-CAPTURE/CAPTURE-THESE.md` — live-app/login shots only (sheep-app, medmac-website + Lighthouse, optiona