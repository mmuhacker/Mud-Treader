<div align="center">

🌟 مدارك تريدر برو

بوت التداول الذكي المتكامل

───


[![by](https://img.shields.io/badge/mmuhacker-%EF%BA%97%EF%BB%84%EF%BB%AE%EF%BB%B3%EF%BA%AE-blue?style=for-the-badge&logo=github)](https://github.com/mmuhacker)<br>
![Version](https://img.shields.io/badge/1.0-%EF%BA%8D%EF%BB%B9%EF%BA%BB%EF%BA%AA%EF%BA%8D%EF%BA%AE-blue?style=for-the-badge)<br>
![Platform](https://img.shields.io/badge/%EF%BB%9B%EF%BA%8E%EF%BB%9F%EF%BB%B2%20%EF%BB%9F%EF%BB%B4%EF%BB%A8%EF%BB%9C%EF%BA%B2-%EF%BA%8D%EF%BB%9F%EF%BA%92%EF%BB%B4%EF%BA%8C%EF%BA%94-green?style=for-the-badge&logo=kalilinux)<br>
![Platform](https://img.shields.io/badge/%EF%BA%84%EF%BB%A7%EF%BA%AA%EF%BA%AE%EF%BB%AE%EF%BB%B3%EF%BA%AA-%EF%BA%8D%EF%BB%9F%EF%BA%92%EF%BB%B4%EF%BA%8C%EF%BA%94-green?style=for-the-badge&logo=android)<br>
![Python](https://img.shields.io/badge/3.x-%EF%BA%91%EF%BA%8E%EF%BB%B3%EF%BA%9C%EF%BB%AE%EF%BB%A6-blue?style=for-the-badge&logo=python)<br>
![License](https://img.shields.io/badge/%EF%BA%97%EF%BA%A0%EF%BA%8E%EF%BA%AD%D9%8A-%EF%BA%8D%EF%BB%9F%EF%BA%98%EF%BA%AE%EF%BA%A7%EF%BB%B4%EF%BA%BA-red?style=for-the-badge)<br>
![Status](https://img.shields.io/badge/%EF%BB%A7%EF%BA%B8%EF%BB%82-%EF%BA%8D%EF%BB%9F%EF%BA%A4%EF%BA%8E%EF%BB%9F%EF%BA%94-blue?style=for-the-badge)


───

📋 المحتويات

</div>

- [المميزات](#-المميزات)
• متطلبات التشغيل
• التثبيت على Termux
• التثبيت على Kali Linux
• المشاكل الشائعة والحلول
• التشغيل
• تحديث الأداة
• التثبيت بأمر واحد
• نظام الترخيص
• المنصات المدعومة
• استخراج التوكن
• شرح القوائم
• الفريم الزمني
• الأسواق المتاحة
• الاستراتيجيات
• قوة الإشارة
• لوحة التحكم
• اختصار التشغيل
• دعم العملات المتعددة
• أخبار السوق
• التنبيهات الصوتية
• المطور

───

<div align="center">

✨ المميزات


الفئة
الميزات

🔗 المنصات
Deriv, Binance, MetaTrader 5, TradingView Webhook

💱 العملات
21 عملة دولية (USD, EUR, GBP, JOD, AED, SAR, QAR, KWD, BHD, OMR, YER, SDG, DZD, LYD, TND, MAD, IQD, SYP, LBP, EGP, TRY)

🎯 الاستراتيجيات
RSI+MA, MACD, Bollinger Bands, دعم/مقاومة, مجمّع

📊 قوة الإشارة
4 مستويات (65%-80%)

🔊 التنبيهات
صوتية للإشارات والأرباح والخسائر

📰 الأخبار
تحديثات مباشرة للسوق

⏱ الفريمات
5 أطر زمنية (1د - 60د)

🔒 الترخيص
نظام متكامل يعمل بدون إنترنت

🎨 الواجهة
عربية بالكامل مع ألوان احترافية

📊 اللوحة
شاشة تحكم متكاملة في الوقت الفعلي

💾 الحفظ
تلقائي للإعدادات والتوكنات

🖥️ البيئة
Termux (Android) + Kali Linux



───

✅ متطلبات التشغيل


المكتبة
الوصف

Python 3.7+
لغة البرمجة الأساسية

websocket-client
الاتصال بخادم Deriv

rich
واجهة المستخدم الملونة

arabic-reshaper
تشكيل النص العربي

python-bidi
اتجاه النص من اليمين لليسار



───

🔧 التثبيت على Termux

</div>

الخطوة 1 — تحديث النظام
bash
pkg update && pkg upgrade -y


الخطوة 2 — تثبيت Python والمكتبات الأساسية

bash
pkg install python curl tor -y


الخطوة 3 — تثبيت مجلد الخطوط

bash
mkdir -p ~/.termux


الخطوة 4 — تثبيت الخط العربي

bash
curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf && termux-reload-settings


⚠️ هام: بعد تثبيت الخط، أغلق Termux بالكامل من قائمة التطبيقات وأعد فتحه

الخطوة 5 — تثبيت مكتبات Python

bash
pip install websocket-client rich arabic-reshaper python-bidi


الخطوة 6 — تنزيل الأداة

bash
curl -o $`PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py


الخطوة 7 — إعطاء صلاحية التشغيل

bash
chmod +x `$PREFIX/bin/mud_tr.py


الخطوة 8 — إنشاء اختصار

bash
ln -sf $`PREFIX/bin/mud_tr.py `$PREFIX/bin/tr


───

<div align="center">

🐉 التثبيت على Kali Linux

</div>

الخطوة 1 — تحديث النظام

bash
sudo apt update && sudo apt upgrade -y


الخطوة 2 — تثبيت Python والمكتبات

bash
sudo apt install python3 python3-pip beep -y


الخطوة 3 — تثبيت مكتبات Python

bash
pip3 install websocket-client rich arabic-reshaper python-bidi


ملاحظة: إذا ظهر خطأ externally-managed-environment، استخدم:

bash
pip3 install websocket-client rich arabic-reshaper python-bidi --break-system-packages


الخطوة 4 — تنزيل الأداة

bash
cd ~
curl -o mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py


الخطوة 5 — إعطاء صلاحية التشغيل

bash
chmod +x mud_tr.py


الخطوة 6 — إنشاء اختصار

bash
sudo ln -sf ~/mud_tr.py /usr/local/bin/tr


───

<div align="center">

⚠️ المشاكل الشائعة والحلول

Termux

</div>

المشكلة الحل
خطأ: pkg: command not found تأكد من تثبيت Termux من F-Droid وليس من Google Play
خطأ: Connection reset by peer جرب تغيير المرآة: termux-change-repo ثم اختر Mirror group
خطأ: Permission denied نفّذ termux-setup-storage وأعد تشغيل Termux
خطأ: النص العربي معكوس ثبّت الخط العربي وأعد تشغيل Termux بالكامل
خطأ: No module named 'rich' pip install rich
خطأ: ModuleNotFoundError: No module named 'websocket' pip install websocket-client
خطأ: pip: command not found pkg install python -y
خطأ: tor: command not found pkg install tor -y
خطأ: beep: command not found التنبيهات الصوتية اختيارية، يمكن تجاهلها
خطأ: Killed أثناء التثبيت المساحة غير كافية، احذف ملفات غير ضرورية: pkg clean

Kali Linux

المشكلة الحل
externally-managed-environment استخدم --break-system-packages
pip3: command not found sudo apt install python3-pip -y
ModuleNotFoundError pip3 install <module_name> --break-system-packages
الخط العربي لا يعمل sudo apt install fonts-noto-core -y

───

<div align="center">

🚀 التشغيل

</div>

بالاختصار (تم إعداده مسبقاً)

bash
tr


أو بالأمر الكامل (Termux)

bash
python $`PREFIX/bin/mud_tr.py


أو بالأمر الكامل (Kali)

bash
python3 ~/mud_tr.py


───

<div align="center">

🔄 تحديث الأداة

</div>

Termux:

bash
curl -o `$PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py && chmod +x $`PREFIX/bin/mud_tr.py


Kali Linux:

bash
cd ~ && curl -o mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py && chmod +x mud_tr.py


───

<div align="center">

⚡ التثبيت بأمر واحد (Termux)

</div>

bash
pkg update && pkg upgrade -y && pkg install python curl -y && pip install websocket-client rich arabic-reshaper python-bidi && curl -o `$PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py && chmod +x $`PREFIX/bin/mud_tr.py && ln -sf `$PREFIX/bin/mud_tr.py $`PREFIX/bin/tr && mkdir -p ~/.termux && curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf && termux-reload-settings && echo "تم تثبيت Mud-Treader (tr) والخط العربي بنجاح!"


───

<div align="center">

🔑 نظام الترخيص

</div>

عند أول تشغيل يطلب البوت مفتاح ترخيص.

للحصول على مفتاح: تواصل مع المطور.

<div align="center">

https://img.shields.io/badge/%EF%BA%97%EF%BB%A4%EF%BA%8D%EF%BA%BB%EF%BB%A0%20%EF%BB%A3%EF%BB%8C%EF%BB%A8%EF%BA%8E-black?style=for-the-badge&logo=gmail&logoColor=red

📸 طلب مفتاح الترخيص

<img src="images/01.png"
width="80%"
style="border-radius: 20px;
border: 2px solid var(--color-border-default);
background: var(--color-canvas-default);
padding: 5px;">


<i style="color: var(--color-fg-default);">الشكل 1: مفتاح الترخيص</i>

مميزات نظام الترخيص:

</div>

· ✅ التحقق التلقائي عبر الإنترنت
· ✅ يعمل بدون إنترنت بعد أول تفعيل
· ✅ يتوقف تلقائياً عند انتهاء الصلاحية
· ✅ 3 محاولات إدخال فقط

───

<div align="center">

## 🏦 المنصات المدعومة

|#|المنصة| النوع| الأسواق|
|---|-----|------|
|1|Deriv| |فوركس + خيارات ثنائية + مؤشرات| 9 أسواق
Binance كريبتو 9 أزواج
MetaTrader 5 فوركس + ذهب + نفط + مؤشرات 9 أسواق
TradingView Webhook إشارات خارجية 5 أسواق

───

## 🔐 استخراج التوكن

**Deriv**

</div>

1. سجّل دخولك على deriv.com
2. اذهب إلى الإعدادات (Settings)
3. اختر Security & Safety
4. اختر API Token
5. اضغط Create new token
6. اختر صلاحية Read و Trade
7. انسخ التوكن الظاهر

**مثال: uYgU8m4B3vXvE8z**

<div align="center">

📷 **توكن ديريف**

<img src="images/04.png"
width="80%"
style="border-radius: 20px;
border: 2px solid var(--color-border-default);
background: var(--color-canvas-default);
padding: 5px;">


<i style="color: var(--color-fg-default);">الشكل 2: توكن ديريف</i>

───

Binance

</div>

1. سجّل دخولك على binance.com
2. اضغط على صورة ملفك الشخصي
3. اختر API Management
4. اضغط Create API
5. اختر System generated
6. أدخل اسماً واضغط Next
7. أكمل التحقق الأمني
8. انسخ API Key

⚠️ ملاحظة: احفظ الـ Secret Key فوراً لأنه لن يظهر مجدداً

<div align="center">

📷 **توكن بينانس**

<img src="images/06.png"
width="80%"
style="border-radius: 20px;
border: 2px solid var(--color-border-default);
background: var(--color-canvas-default);
padding: 5px;">


<i style="color: var(--color-fg-default);">الشكل 3: توكن بينانس</i>

───

**MetaTrader 5**

</div>

1. افتح تطبيق MetaTrader 5
2. اذهب إلى Tools ← Options
3. اختر تبويب Server
4. انسخ رقم Login
5. أدخله في البوت عند الطلب

<div align="center">

📷 **توكن ميتا تريدر**

<img src="images/07.png"
width="80%"
style="border-radius: 20px;
border: 2px solid var(--color-border-default);
background: var(--color-canvas-default);
padding: 5px;">


<i style="color: var(--color-fg-default);">الشكل 4: توكن ميتا تريدر</i>

───

## 📱 شرح القوائم

</div>

الصفحة الرئيسية

1 → تشغيل البوت
2 → الإعدادات
3 → إغلاق البرنامج


<div align="center">

📷 **الصفحة الرئيسية**

<img src="images/02.png"
width="80%"
style="border-radius: 20px;
border: 2px solid var(--color-border-default);
background: var(--color-canvas-default);
padding: 5px;">


<i style="color: var(--color-fg-default);">الشكل 5: الصفحة الرئيسية</i>

</div>

───

<div align="center">

## قائمة الإعدادات (6 خطوات)

|الخطوة| الخيارات|
|1 - المنصة| 1-4 للاختيار، 0 للرئيسية|
|2 - التوكن| إدخال التوكن، c للعملة، 0 للسابق، x للرئيسية|
|3 - العملة |1-21 للاختيار، 0 للسابق|
|4 - السوق |1-9 للاختيار، 0 للسابق، x للرئيسية|
|5 - الاستراتيجية| 1-5 للاختيار، 0 للسابق، x للرئيسية|
|6 - إعدادات الصفقة| المبلغ والمدة، 0 للسابق، x للرئيسية|

</div>

أثناء التشغيل

Ctrl + C → فتح قائمة التحكم

<div align="center">

**قائمة التحكم**
</div>

1 → متابعة تشغيل البوت
2 → تغيير الإعدادات
3 → إغلاق البرنامج


───

<div align="center">
  
## ⏱ الفريم الزمني

</div>

كلما كان الفريم أعلى، كانت الدقة أكبر لكن الانتظار أطول قبل أول صفقة

<div align="center">

|#|الفريم| الانتظار قبل أول صفقة| الوصف|
|---|-----|--------|
|1 |1 دقيقة| ~27 دقيقة| سريع - مناسب للمضاربة السريعة|
|2 |5 دقائق| ~135 دقيقة| متوازن - الأكثر استخداماً|
|3 |10 دقائق| ~270 دقيقة| جيد - دقة معقولة|
|4 |30 دقيقة| ~13 ساعة| محافظ - دقة عالية|
|5 |ساعة |~27 ساعة |آمن جداً - دقة عالية جداً|

───

## 📍 الأسواق المتاحة

**Deriv**

|#|الزوج| النوع|
|---|------|----|
|1 |EUR/USD| فوركس|
|2 |GBP/USD| فوركس|
|3 |USD/JPY| فوركس|
|4| AUD/USD| فوركس|
|5 |USD/CAD| فوركس|
|6| EUR/GBP| فوركس|
|7| مؤشر تقلب 100| مؤشرات|
|8 |مؤشر تقلب 75| مؤشرات|
|9| مؤشر تقلب 50| مؤشرات|

───

**Binance**

|#|الزوج| النوع|
|---|------|----|
|1 |BTC/USDT| كريبتو|
|2 |ETH/USDT| كريبتو|
|3| BNB/USDT| كريبتو|
|4| SOL/USDT| كريبتو|
|5 |XRP/USDT| كريبتو|
|6| ADA/USDT| كريبتو|
|7| DOGE/USDT| كريبتو|
|8| MATIC/USDT| كريبتو|
|9| LTC/USDT| كريبتو|

───

**MetaTrader 5**

|#|الزوج| النوع|
|---|------|----|
|1 |EUR/USD| فوركس|
|2 |GBP/USD| فوركس|
|3 |USD/JPY| فوركس|
|4 |AUD/USD| فوركس|
|5 |USD/CAD| فوركس|
|6 |EUR/GBP| فوركس|
|7 |XAU/USD| ذهب|
|8| النفط الخام| سلع|
|9 |داو جونز| مؤشرات|

───

## 🎯 الاستراتيجيات

|#|الاستراتيجية |الوصف|
|---|------|----------|
|1 |RSI + MA| مؤشر القوة النسبية مع المتوسط المتحرك|
|2 |MACD| تقاطع المتوسطات الأسية|
|3 |Bollinger Bands| نطاقات بولينجر العلوية والسفلية|
|4| دعم ومقاومة| أعلى وأدنى سعر في 20 شمعة|
|5 |مجمّع ⭐ |كل الاستراتيجيات معاً - الأدق|

───

##💪 قوة الإشارة

|#|النسبة| الوصف|
|---|----|--------|
|1| 65% |متوازن - صفقات كثيرة، مخاطرة متوسطة|
|2| 70% |جيد - صفقات معقولة، مخاطرة منخفضة|
|3 |75% |محافظ - صفقات أقل، دقة عالية|
|4 |80%| آمن جداً - صفقات نادرة، دقة عالية جداً|

───

## 📊 لوحة التحكم

|العنصر| الوصف|
|------|----------|
|🤖 الحالة |آخر حدث في البوت|
|🏦 المنصة| المنصة المختارة|
|📍 السوق| الزوج المختار|
|🎯 الاستراتيجية| الاستراتيجية النشطة|
|💱 العملة |العملة الأساسية للعرض|
|💰 الرصيد |رصيد الحساب|
|📈 الربح |صافي الربح/الخسارة|
|📊 المؤشرات| RSI, MA, MACD, BB, دعم/مقاومة|
|⚡ الإشارة| توصية الشراء أو البيع|
|💪 قوة الإشارة| شريط من 0% إلى 100%|
💵 السعر| السعر الفوري المباشر|

───

## ألوان الإشارة

|اللون| المعنى|
|----|--------|
|🟢 أخضر |شراء قوي - صعود مؤكد|
|🔵 أزرق |شراء متوسط - صعود محتمل|
|🔴 أحمر |بيع قوي - هبوط مؤكد|
|🟠 برتقالي |بيع متوسط - هبوط محتمل|
|⏳ أبيض| انتظار - لا فرصة حالياً|

</div>

───

<div align="center">

💱 دعم العملات المتعددة

</div>

يدعم البوت 21 عملة لعرض الرصيد والأرباح:

<div align="center">

| # | العملة | الرمز | الاسم |
|---|----|----|--------|
| 1 | USD |`$ | دولار أمريكي |
| 2 | EUR | € | يورو |
| 3 | GBP | £ | جنيه إسترليني |
| 4 | JOD | JD | دينار أردني |
| 5 | AED | د.إ | درهم إماراتي |
| 6 | SAR | ﷼ | ريال سعودي | 
| 7 | QAR | ﷼ | ريال قطري |
| 8 | KWD | د.ك | دينار كويتي |
| 9 | BHD | د.ب | دينار بحريني |
| 10 | OMR | ر.ع | ريال عُماني |
| 11 | YER | ر.ي | ريال يمني |
| 12 | SDG | ج.س | جنيه سوداني |
| 13 | DZD | د.ج | دينار جزائري |
| 14 | LYD | ل.د | دينار ليبي |
| 15 | TND | د.ت | دبنار تونسي |
| 16 | MAD | د.م | درهم مغربي |
| 17 | IQD|د.ع|دينار عراقي|
|18 |SYP|ل.س|ليرة سورية|
|19| LBP| ل.ل| ليرة لبنانية|
|20| EGP| ج.م|جنيه مصري|
|21 |TRY| ₺| ليرة تركية|

</div>

💡 لتغيير العملة: أثناء إدخال التوكن، اضغط c ثم اختر رقم العملة من القائمة

───

<div align="center">

## 📰 أخبار السوق

</div>

يعرض البوت آخر الأخبار الاقتصادية في لوحة التحكم مباشرة، بما في ذلك:

· 🔴 أخبار عالية التأثير (قرارات الفائدة، بيانات البطالة)
· 🟡 أخبار متوسطة التأثير (مبيعات التجزئة، الإنتاج الصناعي)
· ⚪ أخبار منخفضة التأثير (تصريحات المسؤولين)

📌 يتم تحديث الأخبار تلقائياً كل دقيقة

───

<div align="center">

## 🔊 التنبيهات الصوتية

الحدث الصوت الوصف
🔔 إشارة جديدة تنبيه واحد عند ظهور إشارة قوية (≥65%)
🎉 صفقة رابحة تنبيهان عند إغلاق صفقة بربح
❌ صفقة خاسرة ثلاثة تنبيهات عند إغلاق صفقة بخسارة

</div>

───

<div align="center">

## 🔧 اختصار التشغيل

Termux:

```bash
ln -sf $`PREFIX/bin/mud_tr.py `$PREFIX/bin/tr
```

Kali Linux:

```bash
sudo ln -sf ~/mud_tr.py /usr/local/bin/tr
```

</div>

للتشغيل: اكتب tr واضغط Enter

───

⚠️ تنبيه

⚠️ التداول ينطوي على مخاطر عالية. لا تستثمر أكثر مما تستطيع تحمل خسارته. هذه الأداة لأغراض تعليمية فقط.

───

<div align="center">

## 👨‍💻 المطور

**Muhannad Daher**

[![GitHub](https://img.shields.io/badge/GitHub-mmuhacker-black?style=for-the-badge&logo=github)](https://github.com/mmuhacker)<br>

[![Contact Us](https://img.shields.io/badge/%EF%BA%97%EF%BB%A4%EF%BA%8D%EF%BA%BB%EF%BB%A0%20%EF%BB%A3%EF%BB%8C%EF%BB%A8%EF%BA%8E-black?style=for-the-badge&logo=gmail&logoColor=red)](mailto:madarik.ai.info@gmail.com)

</div>

───

· بوت التداول الذكي
· البيئة: Termux (Android) / Kali Linux
· الإصدار: v2.0
· الترخيص: تجاري

───
<div align="center">

**Madarik Tools — صُنع بالعربية**

⭐ **إذا أعجبتك الأداة، لا تنسَ النجمة!** ⭐

</div>
