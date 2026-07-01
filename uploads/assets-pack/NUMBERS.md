# NUMBERS.md — every figure → its source

**Rule (yours, kept):** if a number isn't in this file with a source, it doesn't go on screen.
**Compiled:** 2026-07-01, by Cowork, from Mohamed's own files.
**Primary sources** (all local, all real):
- `flagship-rebuild/src/data/profile.ts` — the repo's single source of truth for public-safe figures.
- `flagship-rebuild/src/data/projects.ts` — verbatim story stats.
- `flagship-rebuild/src/components/work/*.astro` — the verbatim EN/AR copy + honest-framing lines.
- `CRM latest.xlsx` — the real 12-tab CRM (you uploaded it 2026-06-30).
- `Medmac_Master_Tracker (1) (1).xlsx` + `Suggestions 2026-06-25.xlsx` — the real HR tracker + scoring.

Legend: ✅ verified in a file · ⚠️ NOT in any file yet (do not display until a screenshot/source confirms it).

---

## meta-ads — 2026 paid-social pilot
| Figure | Value | Source |
|---|---|---|
| Cost per WhatsApp lead (avg) | **$0.84** | profile.ts `metaPilot.costPerLeadUsd` ✅ |
| Leads / conversations | **206** | profile.ts `metaPilot.leads` ✅ |
| Total ad spend | **$172.78** | profile.ts `metaPilot.spendUsd` ✅ |
| Best campaign / lead | **$0.50** (Misting Fan · 106 leads) | profile.ts `bestCostPerLeadUsd` + MetaAds.astro ✅ |
| Worst ad (caught + cut) | **$6.25 / call** | MetaAds.astro beat copy ✅ |
| Impressions | **85,132** | profile.ts `metaPilot.impressions` ✅ |
| Reach | **40,460** | profile.ts `metaPilot.reach` ✅ |
| CPM | **$2.03** | CRM `📊 إعلانات ميتا` sheet ✅ (also = 172.78/85,132×1000) |
| CPC | **$0.31** | CRM `📊 إعلانات ميتا` sheet ✅ |
| Frequency | **2.1** | CRM `📊 إعلانات ميتا` sheet ✅ |
| **CTR 0.65%** | **0.65%** | ✅ NOW SOURCED — CRM `📊 إعلانات ميتا` sheet (self-logged from the Meta export). See `crm/` + `meta-ads/meta-metrics-from-crm.png`. Safe to display. |
| Per-campaign | $0.50→106→$52.66 (Misting Fan) · $1.35→28→$37.71 · $1.14→72→$82.41 | CRM `📊 إعلانات ميتا` ✅ |
| By country | Kuwait 170 leads/$150.12 · Iraq 36/$77.66 | CRM `🔗 ربط` / dashboard ✅ |
| Pilot window | **1 May – 3 Jun 2026** | MetaAds.astro + CRM Meta sheet title ✅ |
| Prior period 2024–2025 | ~793K impressions · 214 calls · ~$3.12/call | MetaAds.astro honesty note (self-reported) ✅ |
| Cumulative 2025–2026 | ≈878K impressions · 420+ leads/calls · $0.84–$3.12/lead | profile.ts `cumulative` ✅ |

## al-maali — audience growth (2021–2025)
| Figure | Value | Source |
|---|---|---|
| Facebook | **9.2K → 1M+** | profile.ts `almaali.channels[Facebook]` ✅ |
| Instagram | **3K → 50K** | profile.ts ✅ |
| TikTok | **0 → 33K** | profile.ts ✅ |
| YouTube | **0 → 43K** | profile.ts ✅ |
| Period | **2021–2025** (concluded 2025) | profile.ts + AlMaali.astro honesty ✅ |
| **Follower counts over time (monthly/quarterly series)** | — | ⚠️ DOES NOT EXIST in the files. Only the start/end endpoints above are verified. The yearly **ad-spend** summaries (2022, 2023, 2024, 2025) exist as real screenshots but measure **reach/spend, not followers** — do not relabel them as follower counts. Animate the climb between the two verified endpoints; don't invent in-between follower numbers. |

## crm — 12-tab bilingual CRM
| Figure | Value | Source |
|---|---|---|
| Tabs | **12** | profile.ts `crm.tabs` + real file has exactly 12 sheets ✅ |
| Active named leads | **45** | profile.ts `crm.activeLeads` ✅ |
| Offers sent | **22** | profile.ts `crm.offersRouted` ✅ |
| Contacts captured | **200+** | profile.ts `crm.contactsCaptured` ✅ |
| Closed sales | **0** (correct — see honest line) | CRM `سجل المبيعات` total = 0 ✅ |
| 12 real tab names | لوحة التحكم · مهام اليوم · العملاء · سجل المبيعات · قائمة الأسعار · القوائم · ميستنج · سقالات معلقة · متابعة لاحقاً · 📊 إعلانات ميتا · 🔗 ربط الإعلان بالعملاء · ⚖️ المسؤولية والتأخير | `CRM latest.xlsx` sheet list ✅ |

## sheep-app — desktop software
| Figure | Value | Source |
|---|---|---|
| Tests passing | **59 / 59** (59 assertions, 17 groups, 0 failures) | projects.ts + SheepApp.astro ✅ |
| SQLite tables | **15** | SheepApp.astro ✅ |
| Lines of code | **~2,405** | SheepApp.astro ✅ |
| Successful CI builds | **17** | SheepApp.astro ✅ |
| Build targets | Win10/11 64-bit + Win7 32-bit + macOS (GitHub Actions) | SheepApp.astro ✅ |
| Stack | Python · SQLite · CI | projects.ts ✅ |
| Bug caught in review | vaccination-renewal data-loss, pre-ship | SheepApp.astro ✅ |

## hr-system — recruitment automation
| Figure | Value | Source |
|---|---|---|
| Funnel | **142 parsed → 100 deduped → 8 shortlisted** | HrSystem.astro `funnel` ✅ (8 also traceable to Master Tracker shortlist) |
| Python scripts | **7** | HrSystem.astro ✅ |
| Scheduled jobs live | **3** | HrSystem.astro ✅ |
| Daily cycle | 08:30 intake · WhatsApp read-only every 5h · 19:30 archive | HrSystem.astro ✅ |
| Build date | 24 Jun 2026 (Gmail + WhatsApp + file drops) | HrSystem.astro ✅ |
| Mis-rankings corrected | at least 3 | HrSystem.astro ✅ |

## medmac-website — live on Vercel
| Figure | Value | Source |
|---|---|---|
| Lighthouse | **Performance 96 · Accessibility 100 · Best-Practices 100 · SEO 100** (mobile 96–98) | MedmacWebsite.astro ✅ — re-confirm with a live run (see medmac-website/data.md) |
| Localized page templates | 10 (+404) | MedmacWebsite.astro ✅ |
| Components | ~16 | MedmacWebsite.astro ✅ |
| Commits to production | ~23 | MedmacWebsite.astro ✅ |
| medmac-ui design system | 9-component React + Storybook | MedmacWebsite.astro ✅ |
| Stack | Astro · TypeScript · Tailwind · sharp · Vercel | MedmacWebsite.astro ✅ |
| Live URL | medmac-kuwait.vercel.app | screenshot-checklist.html + checklist ✅ (confirm live) |

## ai-workflow — AI operating model
| Figure | Value | Source |
|---|---|---|
| RFQs consolidated | **23** | projects.ts + AiWorkflow.astro ✅ |
| Reply drafts written | **23** | AiWorkflow.astro ✅ |
| Live tenders recovered | **4** | projects.ts + AiWorkflow.astro ✅ |
| Email scanned | 6 months | AiWorkflow.astro ✅ |
| The 3 AI tools | **Cowork** (controller/memory/briefs) · **Claude Design** (look) · **Claude Code** (build · git · deploy) | AiWorkflow.astro ✅ |

## brand-system — keep CONCEPTUAL ([SKIP] images)
| Figure | Value | Source |
|---|---|---|
| Production files | **~254** | profile-adjacent / BrandSystem.astro ✅ |
| Videos | **~144** | BrandSystem.astro ✅ |
| Brand preview pages | 18 | BrandSystem.astro ✅ |
| Print catalog | 10-page A4 | BrandSystem.astro ✅ |
| Covered | social-ad kits, WhatsApp catalog, OpenSooq · bilingual | BrandSystem.astro ✅ |

## my-resume — Career OS ([SKIP] screenshots)
| Figure | Value | Source |
|---|---|---|
| Framing | **3 tools · 1 workflow · 1 person** | projects.ts ✅ |
| The 3 tools | Cowork · Claude Design · Claude Code | AiWorkflow.astro ✅ |

---

### ⚠️ Do-not-display list (as of 2026-07-01)
1. **al-maali follower time-series** — no monthly/quarterly data exists. Endpoints only (FB 9.2K→1M etc.). The yearly ad-spend summaries are reach/spend, NOT followers.
2. Any client name, candidate name, phone, email, lead WhatsApp, price/offer value, or project-value figure — all redacted in the screenshots; do not source them from anywhere.
3. Anything not listed in this file with a source.

> Update 2026-07-01: **CTR 0.65% is now sourced** (CRM `📊 إعلانات ميتا` sheet) and removed from this list.
