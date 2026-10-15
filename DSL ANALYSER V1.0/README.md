# DSL ANALYSER V1.0

> محلل خطوط DSL / ADSL / VDSL الاحترافي — الإصدار الأساسي
> **المجلد:** `DSL ANALYSER V1.0/` — **ملف البرومبت:** `DSL ANALYSER V1.0/DSL ANALYSER V1.0.md` (2300 سطر — 34 قسم)

## 📌 ما هو هذا الإصدار؟

**DSL ANALYSER V1.0** هو النسخة الأولى والمستقرة لتحليل خطوط النحاس:

- `ADSL / ADSL2 / ADSL2+`
- `VDSL / VDSL2`
- `DSLAM / MSAN`
- تشخيص الزوج النحاسي (Copper Pair) + إعدادات الراوتر/المودم + Wi-Fi والشبكة المنزلية

الفكرة: تنسخ `DSL ANALYSER V1.0/DSL ANALYSER V1.0.md` كاملاً إلى أي مساعد ذكاء اصطناعي (ChatGPT / Claude / Gemini / Copilot / DeepSeek)، ثم ترسل **Screenshot من صفحة DSL Status** أو تلصق القيم كنص، فيحللها كمهندس شبكات ويعطيك تقريراً كاملاً عن السرعة والاستقرار والأخطاء وإمكانية رفع السرعة.

**الهدف:** ليس أعلى رقم Sync فقط، بل **أعلى سرعة عملية ومستقرة** بدون تقطيع أو Re-Sync متكرر.

## 📁 محتويات V1

```
DSL ANALYSER V1.0/
├── DSL ANALYSER V1.0.md   # البرومبت الرئيسي V1.0 — انسخه كاملاً (2300 سطر / 34 قسم)
└── README.md              # هذا الملف — شرح DSL ANALYSER V1.0 المطابق لمحتوى البرومبت الخاص به
```

لا يوجد كود أو تثبيت. كل ما تحتاجه هو ملف `DSL ANALYSER V1.0.md`.

## 🛠️ المتطلبات

1. راوتر **DSL / VDSL** وتعرف الدخول لصفحة إعداداته (عادة `192.168.1.1` — أحياناً `192.168.0.1` أو `192.168.8.1`).
2. حساب على مساعد ذكاء اصطناعي يدعم الصور (GPT-4o أو أحدث / Claude 3.5+ / Gemini 1.5+ / Copilot / DeepSeek).
3. ملف `DSL ANALYSER V1.0/DSL ANALYSER V1.0.md`.
4. Screenshot واضح لصفحة DSL Status.

## 📥 كيف تحصل على بيانات الخط من الراوتر؟

1. افتح المتصفح واكتب `192.168.1.1` وسجّل الدخول (اليوزر/الباسورد غالباً على ظهر الجهاز).
2. ابحث عن:
```
DSL / xDSL / VDSL Status / Line Information / Broadband
```
3. ابحث عن قيم مثل:
```
Sync Rate • SNR Margin • Attenuation • CRC • FEC • Uptime • Attainable Rate
```
4. التقط **Screenshot كامل** بدون قص الأخطاء ومدة التشغيل (Uptime).

**نصائح لصورة جيدة:**
- استخدم متصفح الكمبيوتر وكبّر الصفحة (`Ctrl +`).
- صوّر Downstream و Upstream معاً (ولو في تبويبين صوّر الاثنين).
- أخفِ: IP العام، يوزر/باسورد، رقم الهاتف، MAC إن ظهروا.

**أماكن شائعة:**

| الراوتر | المسار التقريبي |
|---|---|
| WE / ZTE / Huawei | `Status → DSL / xDSL` أو `Maintain → DSL Information` |
| TP-Link | `Status → DSL` أو `Advanced → Status → DSL` |
| D-Link | `Status → WAN / DSL Status` |
| ASUS | `System Log → DSL Log` |
| أي VDSL | ابحث عن `Broadband, Line Rate, SNR Margin, Attenuation, DSL Uptime, Counters, Statistics` |

## 🚀 طريقة الاستخدام خطوة بخطوة (V1)

1. افتح `DSL ANALYSER V1.0/DSL ANALYSER V1.0.md` وانسخ محتواه كاملاً (2300 سطر — لا تختصر).
2. الصقه في الشات كأول رسالة، وأضف سطر:
```
سأرسل لك الآن صورة بيانات الخط لتحليلها
```
سيرد أنه جاهز.
3. ارفع Screenshot صفحة DSL في نفس المحادثة.
4. اقرأ التقرير (جدول التحليل + الخلاصة + القرار الفني في 6 نقاط).
5. لو طلب بيانات ناقصة (Uptime / ES / SES / Speedtest / قراءة بوقت مختلف) أرسلها ليكمل التحليل.

**بديل بدون صورة — الصق القيم يدوياً:**
```
DSL Mode: VDSL2
Profile: 17a
Downstream Current: 49998 kbps
Upstream Current: 9999 kbps
Downstream Attainable: 62000 kbps
Downstream SNR: 8.5 dB
Downstream Attenuation: 12.3 dB
CRC Down: 240
DSL Uptime: 24 hours
...
```

## 🧠 ماذا يغطي برومبت V1؟ (مطابق لمحتوى DSL ANALYSER V1.0.md)

برومبت V1 مقسّم 34 قسماً — وهذا ما يفعله كل جزء:

| القسم في DSL ANALYSER V1.0.md | الوظيفة |
|---|---|
| الدور | يعمل كمهندس ADSL/VDSL + DSLAM/MSAN + Copper Diagnostics + Wi-Fi |
| 1. قواعد التحليل الأساسية | **لا تخمين إطلاقاً** — فقط القيم الظاهرة، وغير الواضح يكتب `غير واضحة — لا يمكن قراءتها بدقة من الصورة` |
| 2. استخراج بيانات الراوتر | استخراج القيم بالوحدة الأصلية (kbps / Mbps / dB / ms / symbols / seconds / hours)، والتمييز بين Down/Up |
| 3. جدول تحليل الخط | جدول واحد بالترتيب الثابت: DSL Mode, Profile, Current Rate, Attainable Rate, SNR Margin, Attenuation, Power, Data Path, Interleave Depth/Delay, INP, CRC, FEC, HEC, ES/SES, G.INP, Vectoring, Bitswap, SRA, DSL Uptime — **فقط الصفوف الظاهرة فعلاً** |
| 4. تفسير القيم | لكل قيمة: اذكرها كما ظهرت + معناها + اربطها بالباقي + صنّفها Measurement / Calculation / Estimate / Interpretation |
| 5. Current / Actual Rate | يوضح Down/Up Sync وأنها مزامنة CPE↔DSLAM وليست Speedtest |
| 6. Attainable + Headroom | يحسب `Current ÷ Attainable × 100` و `Headroom = Attainable − Current` — مع التنبيه أن Attainable تقدير chipset وليس ضمان شركة، ولا يستخدم 70% كقاعدة رسمية |
| 7. SNR Margin | يربطه بـ Sync + Attainable + CRC + ES/SES + Uptime + INP + Interleaving + G.INP — لا حكم من SNR وحده |
| 8. Line Attenuation | فقد الإشارة — **لا يستنتج المسافة** ولا يحوّل dB→متر إلا لو طلبت صراحة (`Distance Estimate ≈ Attenuation × 72 m` كـ Estimate فقط) |
| 9. Power | يذكر القيمة والاتجاه بدون الحكم عليها منفردة |
| 10. Interleaving | آلية توزيع البيانات — زيادة الحماية مقابل Latency — ليست دليل عطل |
| 11. INP | حماية Impulse Noise — تُفسَّر مع Interleaving/Delay/G.INP/CRC/ES/SES/Uptime |
| 12. CRC | يحسب `CRC/hour = CRC ÷ Uptime بالساعات` (مثال: `240 ÷ 24 = 10 CRC/hour`) كـ Calculation — لا حكم من الرقم المطلق |
| 13. FEC | أخطاء تم تصحيحها — وجودها وحده ليس مشكلة |
| 14. ES / SES | مقياس الاستقرار الزمني — تُربط بـ Uptime، وUptime قصيرة لا يُعمَّم منها |
| 15. G.INP | آلية Retransmission — لا تُعتبر دليل جودة/سوء وحدها |
| 16. Vectoring | تقليل Crosstalk في VDSL — لا تُفترض إن لم تظهر |
| 17. Bitswap | إعادة توزيع Bits بين Tones — وجودها طبيعي |
| 18. SRA | تعديل المعدل بدون Re-Sync عند الدعم — تفعيلها لا يعني رفع تلقائي |
| 19. DSL Uptime | مدة Sync منذ آخر Re-Sync — تُستخدم لتفسير كل العدادات |
| 20. تقييم الجودة | فقط: `Excellent / Good / Acceptable / Needs Investigation` — بدون Score رقمي، وبدون حكم من قراءة واحدة |
| 21. إمكانية رفع السرعة | **قرار واحد فقط:** `يمكن تجربة سرعة أعلى` / `السرعة الحالية مناسبة للاستقرار` / `لا توجد بيانات كافية للحكم` + السبب |
| 22. تحديد المشكلة | احتمالات مصنّفة (داخل المنزل: RJ11/Splitter/كابل داخلي/تمديدات/تداخل كهربائي — خارجية: Copper/Joints/بوكس/كابل خارجي/كابينة — DSLAM/Port/Profile/Interleaving/Vectoring/G.INP — راوتر/Firmware/Chipset) — وبدون دليل يكتب `احتمال غير مثبت من البيانات الحالية` |
| 23. التحسينات المادية | بالترتيب: فحص RJ11 → Splitter → تجربة على Main/Test Point → تقصير كابل DSL → إزالة تمديدات → وصلات → بوكس خارجي → فحص زوج نحاسي → فحص DSLAM/Port → مراجعة Speed/Profile |
| 24. تحسين Wi-Fi | فصل مشكلة DSL عن Wi-Fi — 5GHz للقريب / 2.4GHz للبعيد / Channel مناسب / Firmware موثوق / تجربة Ethernet — تغيير DNS ليس حل Sync |
| 25. الأجهزة والاستهلاك | فحص الأجهزة/التحميلات/التحديثات/Cloud/Streaming/Torrent — QoS يوزّع فقط ولا يرفع سرعة الخط |
| 26. DNS | للـ Resolution وفتح المواقع فقط — فرّق بين DNS latency و Internet latency و DSL performance |
| 27. OS / Device | فحص خلفية/تحديثات/Cloud Sync/إضافات متصفح/Malware/CPU-RAM-Disk/Wi-Fi — لا تنسب بطء الجهاز لـ DSL بدون اختبار |
| 28. Speedtest وPing | فصل DSL Sync عن Throughput و Latency و Wi-Fi — Sync عالٍ + Speedtest منخفض = ابحث في Ethernet/Wi-Fi/CPU/ISP/Congestion/Server/Background/Device |
| 29. عند اقتراح رفع السرعة | يحذّر من: انخفاض SNR، زيادة CRC وES/SES، انخفاض استقرار، Re-Sync، تغيّر Data Path/Interleaving |
| 30. البيانات الناقصة | يطلب فقط اللازم بسبب واضح (Spectrum / SNR per Tone / Bit Loading / Uptime / CRC-ES-SES / Ping / Speedtest / قراءات بأوقات مختلفة) |
| 31. قاعدة الصور | واضحة=استخرج، جزئية=الموثوق فقط، غير واضحة=اكتب العبارة بدون تخمين |
| 32. القرار الفني النهائي | 6 نقاط: حالة DSL / أخطاء؟ / عدم استقرار؟ / Headroom؟ / بيانات كافية لرفع؟ / أهم خطوة تالية؟ |
| 33. الخلاصة | جدول ثابت: الحالة / السرعة / SNR / Attenuation / الأخطاء / الاستقرار / إمكانية الرفع / أهم مشكلة / التحسين / ما لا يمكن إثباته |
| 34. قاعدة التنفيذ | التسلسل الدائم: `استخرج → تحقق → احسب → فسّر → اربط → قيّم → حدد الاحتمالات → اقترح → لخّص` |

## 📊 مخرجات تحليل V1

1. **جدول تحليل الخط** — أعمدة: الخاصية / التعريف البسيط / Download / Upload / ماذا تعني في خطك؟ / الحساب / التقييم / الدليل.
2. **جدول الخلاصة** — الحالة، السرعة (Current مقابل Attainable)، SNR، Attenuation، الأخطاء (+CRC/hour)، الاستقرار، قرار الرفع، أهم مشكلة، التحسين، ما لا يمكن إثباته.
3. **القرار الفني النهائي (6 نقاط)** كما بالأعلى.

معادلات يحسبها لك:
```
نسبة الاستخدام % = (Current ÷ Attainable) × 100
Headroom = Attainable − Current
CRC/hour = عدد CRC ÷ مدة التشغيل بالساعات
```

**مثال:** `40960 ÷ 55000 × 100 = 74.47%` — `Headroom = 14040 kbps ≈ 14 Mbps` — `120 ÷ 48 = 2.5 CRC/hour`

## ⚖️ قواعد V1 الصارمة (ملخص)

- لا تخمين، لا اختراع Mode/Profile/SNR/Attenuation/Errors.
- Speedtest ≠ Sync.
- CRC تُربط بالزمن + ES/SES، وFEC وحده ليس مشكلة.
- Attainable المرتفع ليس ضمان رفع.
- لا اتهام للشركة بدون دليل، ولا تغيير SNR Target/Profile عشوائياً.
- `1 dB = 72 m` ليست قياس مسافة — Estimate عند الطلب فقط.
- التفريق الدائم: Measurement / Calculation / Estimate / Interpretation.

## 🔀 DSL أم Wi-Fi؟

| العرض | غالباً DSL | غالباً Wi-Fi/جهاز |
|---|---|---|
| لمبة DSL تفصل/ترمش | ✅ | ❌ |
| Sync منخفض / CRC مرتفع / Re-Sync متكرر | ✅ | ❌ |
| بطء على كل الأجهزة حتى بالكابل | ✅ | ❌ |
| ممتاز بالكابل وسيئ على الموبايل | ❌ | ✅ |
| Ping عالٍ على Wi-Fi فقط | ❌ | ✅ |

**القاعدة الذهبية:** جهاز واحد بكابل Ethernet وبدون تحميلات، ثم قارن Speedtest مع Sync.

## ❓ أسئلة V1 الشائعة

- **هل أحتاج خبرة؟** لا — انسخ البرومبت وأرسل الصورة واقرأ الخلاصة.
- **الراوتر لا يعرض Attainable أو الأخطاء؟** يعمل — يحلل الظاهر فقط ويكتب الناقص.
- **Speedtest فقط يكفي؟** لا يحدد جودة النحاس — لازم بيانات DSL.
- **VDSL قراءاته مختلفة عن ADSL؟** طبيعي — يراعي التقنية الظاهرة.
- **الخصوصية؟** بيانات DSL ليست حساسة، لكن أخفِ IP العام/يوزر/باسورد/هاتف/MAC.
- **كم مرة أفحص؟** مرة بحالة مستقرة للمقارنة + مرة وقت المشكلة + يفضّل صباحاً ومساءً.

## 🆚 متى تستخدم V1؟

- تريد تحليل DSL أساسي سريع ودقيق بدون تعقيد القوائم.
- أول مرة تفحص خطك.
- **لو تريد تحليل متقدم (Spectrum / Crosstalk / مقارنة زمنية / تقرير ISP للتصعيد / قائمة تفاعلية) → استخدم V2.**
- **لو خطك فايبر (FTTH/GPON) وليس نحاس → استخدم V3.**

> إخلاء مسؤولية: التحليل استرشادي يعتمد على ما ترسله ولا يغني عن الفحص الميداني من الفني/الشركة.
