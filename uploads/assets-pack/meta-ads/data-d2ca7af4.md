# meta-ads — Paid Social · PRIORITY 4

## Verbatim numbers
- **$0.84 / WhatsApp lead** (avg) · **206 leads** · **$172.78 total spend**
- **$0.50** best campaign/lead (Misting Fan · 106 leads) · **$6.25/call** worst ad (caught + cut)
- **85,132 impressions** · **40,460 reach** · **CPM $2.03** · **CPC $0.31** · **CTR 0.65%** · **frequency 2.1**
- Per-campaign: **$0.50 → 106 conv → $52.66** (Misting Fan, best) · $1.35 → 28 → $37.71 · $1.14 → 72 → $82.41
- By country: Kuwait 170 leads / $150.12 · Iraq 36 / $77.66
- Pilot window **1 May – 3 Jun 2026** · conversion noted in-sheet: 1$ ≈ 0.307 KWD
- Prior 2024–2025 (self-reported): ~793K impressions · 214 calls · ~$3.12/call
- Cumulative 2025–2026: ≈878K impressions · 420+ leads/calls
- Source: `profile.ts → metaPilot / cumulative` + `MetaAds.astro` + **CRM `📊 إعلانات ميتا` sheet** (the live ad snapshot).

## ✅ CTR 0.65% — now confirmed
CTR 0.65% (with CPC $0.31, CPM $2.03, frequency 2.1) **is in the CRM's `📊 إعلانات ميتا` sheet** — see `meta-metrics-from-crm.png`. It's self-logged from the Meta export (same basis as the rest of the pilot reporting), so it's safe to display.

## Copy to reuse (verbatim)
**Hero** — EN: "Leads under **a dollar**." · AR: «عملاء بأقلّ **من دولار**.»
**Lead** — EN: "A measured Meta pilot for a B2B industrial supplier: I turned $172.78 of spend into 206 WhatsApp conversations — at about **$0.84 each**." · AR: «تجربة ميتا مُقاسة لمورّد صناعي B2B: حوّلت إنفاقًا قدره ١٧٢٫٧٨$ إلى ٢٠٦ محادثة واتساب — بنحو **٠٫٨٤$ للواحدة**.»
**Honest line (verbatim)** — EN: "The numbers above are the measured 2026 pilot (1 May–3 Jun) from the live CRM. I generate the leads — the company's engineer prices and closes — so I report leads, not closed revenue. An earlier 2024–2025 period self-reports ~793K impressions and 214 calls at ~$3.12 each; combined, ≈878K impressions and 420+ leads." · AR: «الأرقام أعلاه هي تجربة ٢٠٢٦ المُقاسة (١ مايو–٣ يونيو) من نظام العملاء الحيّ. أنا أُولّد العملاء — ومهندس الشركة يُسعّر ويُغلق — لذا أُبلّغ عن العملاء لا عن الإيرادات المُغلقة. وفي فترة سابقة ٢٠٢٤–٢٠٢٥ يذكر تصدير إعلاناتي ذاتيًا نحو ٧٩٣ ألف ظهور و٢١٤ مكالمة بنحو ٣٫١٢$ للواحدة؛ ومجتمعةً نحو ٨٧٨ ألف ظهور و٤٢٠+ عميلًا.»

## Screenshots in this folder
- `meta-metrics-from-crm.png` — ✅ the real Meta snapshot from the CRM (CPC 0.31 / CPM 2.03 / **CTR 0.65%** / $0.84 cost-per-conv / 206 / freq 2.1 / 85,132 imp / 40,460 reach) + per-campaign + by-country tables. The honest, sourced numbers panel.
- `creatives/*.png|jpg` — real ad creatives (Heavy Equipment, Scaffolding, ad-5). ✅ real, cleared.
- `img-work-labels.md` — labels for the 8 existing `public/img/work/*.jpg` (what each shows + real/usable).
- [NICE, pending] `ads-manager.png` — a native Meta Ads Manager results view (cosmetic; the numbers are already in `meta-metrics-from-crm.png`). **Your login only** — see `_TO-CAPTURE/`.
- [NICE, pending] `click-to-whatsapp.png` — a click-to-WhatsApp ad in the wild.
