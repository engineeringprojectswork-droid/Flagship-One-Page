# hr-system — Automation

## Verbatim numbers
- Funnel **142 parsed → 100 deduped → 8 shortlisted**
- **7** Python scripts · **3** scheduled jobs live
- Daily cycle: **08:30** intake · read-only WhatsApp check **every 5h** · **19:30** archive
- Build date: **24 Jun 2026** (Gmail + WhatsApp + file drops); corrected ≥3 mis-rankings
- Source: `HrSystem.astro`. The 8-shortlist + scoring also trace to `Medmac_Master_Tracker.xlsx` / `Suggestions 2026-06-25.xlsx`.

## Copy to reuse (verbatim)
**Hero** — EN: "Hiring on **autopilot**." · AR: «توظيفٌ **يعمل تلقائيًا**.»
**Lead** — EN: "Résumés arrive on three channels at once. **7 Python scripts and 3 scheduled jobs** collect, dedupe, read-score and track them daily — and never message a candidate without approval." · AR: «السِّيَر تصل عبر ثلاث قنواتٍ معًا. **٧ سكربتات بايثون و٣ مهام مجدولة** تجمعها وتُزيل التكرار وتُقيّمها بالقراءة وتتتبّعها يوميًا — ولا تراسل مرشّحًا دون موافقة.»
**Honest line** — EN: "Spec-driven, AI-assisted (Claude Code), operated daily by me — I set the roles, the rubric, the rules and the manager-review mode, and I approve every invitation. Time saved and recruiter-fee avoidance were never measured, so they aren't claimed." · AR: «مدفوعٌ بالمواصفات، وبمساعدة الذكاء الاصطناعي (Claude Code)، وأُشغّله يوميًا — وضعت الأدوار والمعايير والقواعد ووضع مراجعة المدير، وأوافق على كل دعوة. ولم يُقَس الوقت الموفّر ولا توفير أتعاب التوظيف، فلا يُدّعيان.»

## Screenshots in this folder — ✅ DONE (rendered from the real trackers, PII redacted before render)
- `hr-master-tracker.png` — the colour-coded **SHORTLIST** master tracker grouped by role (Sales Engineer, Structural Metal Engineer, Sales & Marketing…), with rating ★, exp, nationality, the **read-verified "WHY" reasoning** (skill-based, no names), interview slots. Candidate **name / phone / email blocked (▇)**; subtitle + excluded-names footer also blanked.
- `hr-all-candidates.png` — the full **ALL CANDIDATES** archive (deduped, ~130 rows) showing role bucket, rating, exp, applied date, source, status (INVITED / EXCLUDED…). Name / phones / emails **blocked**.
- `hr-color-key.png` — the 🎨 colour-key legend (GREEN=confirmed, BLUE=came, YELLOW=invited, RED=rejected, TEAL=hired…). Feeds the pipeline colour story.
- `hr-scoring.png` — the read-verified **scoring** sheet: ROLE / GENDER / **MY SCORE** / **MY REASONING** / decision. Name / phone / email **blocked**; the role-based reasoning (the proof of "read, don't keyword-match") is intact and contains no names.
- [NICE, pending] a scheduled-job log / daily-clock screenshot (your machine) — see `_TO-CAPTURE/`.

**Redaction:** candidate name/phone/email columns blanked in-cell before render; regex safety-net asserted 0 contact-data cells remain; the "male-only policy" note is your real, already-public documented criterion (also in the site copy).
