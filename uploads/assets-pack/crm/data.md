# crm — Marketing Ops · PRIORITY 2

## Verbatim numbers
- **12** bilingual tabs · **45** active named leads · **22** offers sent · **200+** contacts captured · **0** closed sales (correct)
- Source: `profile.ts → crm`; 12 tabs + 0-closed confirmed in the real `CRM latest.xlsx`.

## The 12 real tab names (verbatim, in file order)
1. لوحة التحكم (Dashboard) · 2. مهام اليوم (Today's tasks) · 3. العملاء (Leads/Clients) ·
4. سجل المبيعات (Sales log) · 5. قائمة الأسعار (Price list) · 6. القوائم (Lists + colour key) ·
7. ميستنج (Misting leads) · 8. سقالات معلقة (Scaffolding leads) · 9. متابعة لاحقاً (Follow-up later) ·
10. 📊 إعلانات ميتا (Meta ads snapshot) · 11. 🔗 ربط الإعلان بالعملاء (Ad → lead link) · 12. ⚖️ المسؤولية والتأخير (Accountability / delay)

## Status taxonomy + colours (verbatim labels from Crm.astro)
- **New lead** (عميل جديد) · **Offer sent** (عرض مُرسل · 22) · **High priority** (أولوية عالية · ★) · **→ Engineer** (← المهندس · ↗)
- Colour logic = conditional formatting; the real colour key lives in tab 6 `القوائم` → "🎨 دليل ألوان الحالة".

## Copy to reuse (verbatim)
**Hero** — EN: "From ad spend to a **tracked lead**." · AR: «من الإنفاق إلى **عميلٍ مُتتبَّع**.»
**Lead** — EN: "No system existed, so I built one: a **12-tab bilingual CRM** that connects every dinar of ad spend to a named lead and a next action." · AR: «لم يكن هناك نظام، فبنيت واحدًا: **نظام عملاء ثنائي اللغة من ١٢ تبويبًا** يربط كل دينار إنفاقٍ بعميلٍ مُسمّى وإجراءٍ تالٍ.»
**Honest line** — EN: "The CRM currently shows 0 closed sales — and that's correct: I run marketing and lead-gen; the engineer prices and closes. The system's job is to make sure no lead is lost on the way there." · AR: «يُظهر النظام حاليًا ٠ صفقة مُغلقة — وهذا صحيح: أنا أُدير التسويق وتوليد العملاء؛ والمهندس يُسعّر ويُغلق. ومهمة النظام ألّا يضيع أيُّ عميلٍ في الطريق.»

## Screenshots in this folder — ✅ DONE (rendered from the real `CRM latest.xlsx`, Arabic intact, PII redacted in the data before render)
- `crm-dashboard.png` — tab 1 لوحة التحكم: **207 total contacts**, status/priority/country breakdown, **22 offers, 0 sold** (corroborates the honest line). No PII.
- `crm-leads-tab.png` — tab 3 العملاء: the colour-coded pipeline (priority → status → next action). Name / WhatsApp / full-number / offer-value / notes columns **all blocked (▇)**.
- `crm-ads-to-leads.png` — tab 11 🔗 ربط الإعلان بالعملاء: the ad-spend → leads funnel (product → spend → conversations → CRM leads → offers). Totals 206 / $172.78. No PII (products only).
- `crm-accountability-sla.png` — tab 12 ⚖️ المسؤولية والتأخير: owner-by-role (You / Engineer / Client), day-counter, fault scoring. Embedded client card + name/number **blocked**.
- `crm-status