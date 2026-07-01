# sheep-app — Software · PRIORITY 3

## Verbatim numbers
- **59 / 59** tests passing (59 assertions across 17 groups, 0 failures)
- **15** SQLite tables · **~2,405** lines of code · **17** successful CI builds
- Builds: Win10/11 64-bit + Win7 32-bit + macOS, via GitHub Actions on every push
- Stack: **Python · SQLite · CI**
- Source: `projects.ts` + `SheepApp.astro`.

## Copy to reuse (verbatim)
**Hero** — EN: "Software that **actually ships**." · AR: «برمجيات **تُسلَّم فعلًا**.»
**Lead** — EN: "An offline, bilingual desktop app for a real sheep farm — a 15-table database, a collision-proof identity model, and a decision-support engine, packaged for Windows + macOS and proven by **59/59 automated tests**." · AR: «تطبيق سطح مكتب يعمل دون إنترنت وثنائي اللغة لمزرعة أغنامٍ حقيقية — قاعدة من ١٥ جدولًا، ونموذج هويةٍ مانعٌ للتصادم، ومحرّك دعمٍ للقرار، مُحزَّم لويندوز وماك ومُثبَت بـ٥٩/٥٩ اختبارًا آليًا.»
**The hard problem** — EN: "A data-integrity problem, disguised as a farm app. Ear numbers are reused after an animal is sold or dies — so the whole system had to guarantee old and new records could never blur together, fully offline, Arabic-first." · AR: «مشكلة سلامة بيانات، مُتنكّرة في هيئة تطبيق مزرعة. أرقام الأذن تُعاد بعد بيع الحيوان أو نفوقه — لذا وجب أن يضمن النظام استحالة اختلاط السجلات القديمة بالجديدة، دون إنترنت، وبالعربية أولًا.»
**Honest line** — EN: "Spec-driven, AI-assisted development (Claude Code). I'm the architect, decision-maker, reviewer and operator — I set the no-mixing rule, designed the schema and the three-herd model, ran the adversarial review, and shipped the builds. Business impact (time/money saved) was never measured, so I claim only the delivery facts above." · AR: «تطويرٌ مدفوعٌ بالمواصفات وبمساعدة الذكاء الاصطناعي (Claude Code). أنا المهندس وصاحب القرار والمراجع والمشغّل — وضعت قاعدة عدم الاختلاط، وصمّمت المخطّط ونموذج القطعان الثلاثة، وأجريت المراجعة النقدية، وأطلقت الإصدارات. ولم يُقَس الأثر التجاري، فلا أدّعي سوى حقائق التسليم أعلاه.»

## Schema (verbatim facts — usable as a table list if no diagram)
15 relational SQLite tables; every event foreign-keyed to a specific generation; safe non-destructive migrations on startup; three-herd identity model; ear-number reuse cannot blur old/new records.

## Screenshots in this folder — [REQUIRED]
- `sheep-app-en.png` — main window, English UI. **[pending — needs the app running on your machine]**
- `sheep-app-ar.png` — main window, Arabic UI. **[pending]**
- `sheep-tests-59-59.png` — the 59/59 test run output (terminal or CI). **[pending]**
- `sheep-ci-build.png` — a GitHub Actions successful build (17 builds). **[pending — your GitHub repo]**
- [NICE] app icon, stack confirmation.

> None of these exist as files. They live on your machine / your GitHub. We'll capture the app + test run from your screen; the CI build is one screenshot from your repo's Actions tab. See `_TO-CAPTURE/SHEEP-APP.md`.
