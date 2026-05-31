<div align="center">
  
**🌟 مدارك تريدر برو - V1.0**

*بوت التداول الذكي المتكامل*

---

![Version](https://img.shields.io/badge/1.0-%EF%BA%8D%EF%BB%B9%EF%BA%BB%EF%BA%AA%EF%BA%8D%EF%BA%AE-blue?style=for-the-badge)
![Platform]![Version](https://img.shields.io/badge/1.0-%EF%BA%8D%EF%BB%B9%EF%BA%BB%EF%BA%AA%EF%BA%8D%EF%BA%AE-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Kali_Linux-%EF%BA%8D%EF%BB%9F%EF%BA%92%EF%BB%B4%EF%BA%8C%EF%BA%94-green?style=for-the-badge&logo=kalilinux)
![Platform](https://img.shields.io/badge/Android-%EF%BA%8D%EF%BB%9F%EF%BA%92%EF%BB%B4%EF%BA%8C%EF%BA%94-green?style=for-the-badge&logo=android)
![Python](https://img.shields.io/badge/Python-3.x-yellow?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/Commercial-%EF%BA%8D%EF%BB%9F%EF%BA%98%EF%BA%AE%EF%BA%A7%EF%BB%B4%EF%BA%BC-red?style=for-the-badge)
![Status](https://img.shields.io/badge/%EF%BB%A7%EF%BA%B8%EF%BB%A2-%EF%BA%8D%EF%BB%9F%EF%BA%A4%EF%BA%8E%EF%BB%9F%EF%BA%94-brightgreen?style=for-the-badge)

---

📋 **المحتويات**
</div>

- [متطلبات التشغيل](#-متطلبات-التشغيل)
- [التثبيت](#-التثبيت)
- [التشغيل](#-التشغيل)
- [تحديث الأداة](https://github.com/mmuhacker/Mud-Treader/blob/main/README.md#-%D8%AA%D8%AD%D8%AF%D9%8A%D8%AB-%D8%A7%D9%84%D8%A3%D8%AF%D8%A7%D8%A9)
- [التثبيت بأمر واحد](https://github.com/mmuhacker/Mud-Treader/blob/main/README.md#%D8%A7%D9%84%D8%AA%D8%AB%D8%A8%D9%8A%D8%AA-%D8%A8%D8%A3%D9%85%D8%B1-%D9%88%D8%A7%D8%AD%D8%AF)
- [نظام الترخيص](#-نظام-الترخيص)
- [المنصات المدعومة](#-المنصات-المدعومة)
- [استخراج التوكن](#-استخراج-التوكن)
- [شرح القوائم](#-شرح-القوائم)
- [الفريم الزمني](#-الفريم-الزمني)
- [الأسواق المتاحة](#-الأسواق-المتاحة)
- [الاستراتيجيات](#-الاستراتيجيات)
- [قوة الإشارة](#-قوة-الإشارة)
- [لوحة التحكم](#-لوحة-التحكم)
- [اختصار التشغيل](https://github.com/mmuhacker/Mud-Treader/blob/main/README.md#--%D8%A7%D8%AE%D8%AA%D8%B5%D8%A7%D8%B1-%D8%A7%D9%84%D8%AA%D8%B4%D8%BA%D9%8A%D9%84)
- [المطور](https://github.com/mmuhacker/Mud-Treader/blob/main/README.md#%E2%80%8D-%D8%A7%D9%84%D9%85%D8%B7%D9%88%D8%B1)

---
<div align="center">
  
## ✅ متطلبات التشغيل

| المكتبة | الوصف |
|---------|-------|
| python | لغة البرمجة الأساسية |
| websocket-client | الاتصال بخادم Deriv |
| rich | واجهة المستخدم الملونة |
| arabic-reshaper | تشكيل النص العربي |
| python-bidi==0.4.2 | اتجاه النص من اليمين لليسار |

---

## 🔧 التثبيت
</div>

**1. تحديث النظام والمكتبات وتثبيت المتطلبات (لمرة واحدة)**
```bash
pkg update && pkg upgrade -y && pkg install python curl tor -y && mkdir -p ~/.termux
```

**2. تثبيت الخط العربي (مرة واحدة) إذا لم يكن مثبتاً**
```bash
curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf && termux-reload-settings

```
<div align="center">

## # ⚡ اختصار التشغيل
</div>

**تثبيت المكتبات وإعداد الإختصار**
```bash
pip install arabic-reshaper python-bidi --break-system-packages && curl -o $PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud_Treader/main/mud_tr.py && chmod +x $PREFIX/bin/mud_tr.py && ln -sf $PREFIX/bin/mud_tr.py $PREFIX/bin/tr

```
## 🔄 تحديث الأداة
**يتم تحديث الأداة عند صدور تحديث بهذا الأمر**
```bash
curl -o $PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud_Treader/main/mud_tr.py && chmod +x $PREFIX/bin/mud_tr.py
```

---
<div align="center">

## 🚀 التشغيل
</div>

**بالاختصار (تم إعداده مسبقاً)**
```bash
tr
```

**أو بالأمر الكامل**
```bash
python ~/mud_tr.py
```
<div align="center">
  
## التثبيت بأمر واحد
</div>

**تثبيت المكتبات والمتطلبات والتشغيل بأمر واحد لمرة واحدة**


```bash
pkg update && pkg upgrade -y && pkg install python curl -y && pip install websocket-client rich arabic-reshaper python-bidi==0.4.2 --break-system-packages && curl -o $PREFIX/bin/mud_tr.py https://raw.githubusercontent.com/mmuhacker/Mud-Treader/main/mud_tr.py && chmod +x $PREFIX/bin/mud_tr.py && ln -sf $PREFIX/bin/mud_tr.py $PREFIX/bin/tr && mkdir -p ~/.termux && curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf && termux-reload-settings && echo "تم تثبيت أداة Mud-Treader (tr) والخط العربي بنجاح!"
```


---
<div align="center">
  
## 🔑 نظام الترخيص
</div>
عند أول تشغيل يطلب البوت مفتاح ترخيص.

**للحصول على مفتاح:** تواصل مع المطور.
<div align="center">
  
[![Contact Us](https://img.shields.io/badge/%EF%BA%97%EF%BB%A4%EF%BA%8D%EF%BA%BB%EF%BB%A0%20%EF%BB%A3%EF%BB%8C%EF%BB%A8%EF%BA%8E-black?style=for-the-badge&logo=gmail&logoColor=red)](mailto:madarik.ai.info@gmail.com)


  
**مميزات النظام:**

</div>

- ✅ التحقق التلقائي عبر الإنترنت
- ✅ يعمل بدون إنترنت بعد أول تفعيل
- ✅ يتوقف تلقائياً عند انتهاء الصلاحية
- ✅ 3 محاولات إدخال فقط

---
<div align="center">


## 🏦 المنصات المدعومة

| المنصة | النوع | الأسواق |
|--------|-------|---------|
| **Deriv** | فوركس + خيارات ثنائية + مؤشرات | 9 أسواق |
| **Binance** | كريبتو | 9 أزواج |
| **MetaTrader 5** | فوركس + ذهب + نفط + مؤشرات | 9 أسواق |

---

## 🔐 استخراج التوكن

***Deriv***
</div>

1. سجّل دخولك على [deriv.com](https://deriv.com)
2. اذهب إلى **الإعدادات** (Settings)
3. اختر **Security & Safety**
4. اختر **API Token**
5. اضغط **Create new token**
6. اختر صلاحية **Read** و **Trade**
7. انسخ التوكن الظاهر

> مثال: `uYgU8m4B3vXvE8z`

---
<div align="center">

***Binance***
</div>

1. سجّل دخولك على [binance.com](https://binance.com)
2. اضغط على صورة ملفك الشخصي
3. اختر **API Management**
4. اضغط **Create API**
5. اختر **System generated**
6. أدخل اسماً واضغط **Next**
7. أكمل التحقق الأمني
8. انسخ **API Key**

> ملاحظة: احفظ الـ Secret Key فوراً لأنه لن يظهر مجدداً

---
<div align="center">

***MetaTrader 5***
</div>

1. افتح تطبيق **MetaTrader 5**
2. اذهب إلى **Tools** ← **Options**
3. اختر تبويب **Server**
4. انسخ رقم **Login**
5. أدخله في البوت عند الطلب

---
<div align="center">
  
## 📱 شرح القوائم

### الصفحة الرئيسية
```
1 → تشغيل البوت
2 → الإعدادات
3 → إغلاق البرنامج
```

### قائمة الإعدادات (6 خطوات)

| الخطوة | الخيارات |
|--------|----------|
| 1 - المنصة | 1-3 للاختيار، 0 للرئيسية |
| 2 - التوكن | إدخال التوكن، 0 للسابق، x للرئيسية |
| 3 - السوق | 1-9 للاختيار، 0 للسابق، x للرئيسية |
| 4 - الفريم الزمني | 1-5 للاختيار، 0 للسابق، x للرئيسية |
| 5 - الاستراتيجية | 1-5 للاختيار، 0 للسابق، x للرئيسية |
| 6 - قوة الإشارة | 1-4 للاختيار، 0 للسابق، x للرئيسية |

### أثناء التشغيل
```
Ctrl + C → فتح قائمة التحكم
```

### قائمة التحكم
```
1 → متابعة تشغيل البوت
2 → تغيير الإعدادات
3 → إغلاق البرنامج
```

---

## ⏱ الفريم الزمني

> كلما كان الفريم أعلى، كانت الدقة أكبر لكن الانتظار أطول قبل أول صفقة

| # | الفريم | الانتظار قبل أول صفقة | الوصف |
|---|--------|----------------------|-------|
| 1 | 1 دقيقة | ~27 دقيقة | سريع - مناسب للمضاربة السريعة |
| 2 | 5 دقائق | ~135 دقيقة | متوازن - الأكثر استخداماً |
| 3 | 10 دقائق | ~270 دقيقة | جيد - دقة معقولة |
| 4 | 30 دقيقة | ~13 ساعة | محافظ - دقة عالية |
| 5 | ساعة | ~27 ساعة | آمن جداً - دقة عالية جداً |

---

## 📍 الأسواق المتاحة

**Deriv**
| # | الزوج | النوع |
|---|-------|-------|
| 1 | EUR/USD | فوركس |
| 2 | GBP/USD | فوركس |
| 3 | USD/JPY | فوركس |
| 4 | AUD/USD | فوركس |
| 5 | USD/CAD | فوركس |
| 6 | EUR/GBP | فوركس |
| 7 | مؤشر تقلب 100 | مؤشرات |
| 8 | مؤشر تقلب 75 | مؤشرات |
| 9 | مؤشر تقلب 50 | مؤشرات |

---

**Binance**
| # | الزوج | النوع |
|---|-------|-------|
| 1 | BTC/USDT | كريبتو |
| 2 | ETH/USDT | كريبتو |
| 3 | BNB/USDT | كريبتو |
| 4 | SOL/USDT | كريبتو |
| 5 | XRP/USDT | كريبتو |
| 6 | ADA/USDT | كريبتو |
| 7 | DOGE/USDT | كريبتو |
| 8 | MATIC/USDT | كريبتو |
| 9 | LTC/USDT | كريبتو |

---

**MetaTrader 5**
| # | الزوج | النوع |
|---|-------|-------|
| 1 | EUR/USD | فوركس |
| 2 | GBP/USD | فوركس |
| 3 | USD/JPY | فوركس |
| 4 | AUD/USD | فوركس |
| 5 | USD/CAD | فوركس |
| 6 | EUR/GBP | فوركس |
| 7 | XAU/USD | ذهب |
| 8 | النفط الخام | سلع |
| 9 | داو جونز | مؤشرات |

---

## 🎯 الاستراتيجيات

| # | الاستراتيجية | الوصف |
|---|--------------|-------|
| 1 | RSI + MA | مؤشر القوة النسبية مع المتوسط المتحرك |
| 2 | MACD | تقاطع المتوسطات الأسية |
| 3 | Bollinger Bands | نطاقات بولينجر العلوية والسفلية |
| 4 | دعم ومقاومة | أعلى وأدنى سعر في 20 شمعة |
| 5 | مجمّع ⭐ | كل الاستراتيجيات معاً - الأدق |

---

## 💪 قوة الإشارة

| # | النسبة | الوصف |
|---|--------|-------|
| 1 | 65% | متوازن - صفقات كثيرة، مخاطرة متوسطة |
| 2 | 70% | جيد - صفقات معقولة، مخاطرة منخفضة |
| 3 | 75% | محافظ - صفقات أقل، دقة عالية |
| 4 | 80% | آمن جداً - صفقات نادرة، دقة عالية جداً |

---

## 📊 لوحة التحكم

| العنصر | الوصف |
|--------|-------|
| 🤖 الحالة | آخر حدث في البوت |
| 🏦 المنصة | المنصة المختارة |
| 📍 السوق | الزوج المختار |
| 🎯 الاستراتيجية | الاستراتيجية النشطة |
| 💰 الرصيد | رصيد الحساب |
| 📈 الربح | صافي الربح/الخسارة |
| 📊 المؤشرات | RSI, MA, MACD, BB, دعم/مقاومة |
| ⚡ الإشارة | توصية الشراء أو البيع |
| 💪 قوة الإشارة | شريط من 0% إلى 100% |
| 💵 السعر | السعر الفوري المباشر |

---

### ألوان الإشارة

| اللون | المعنى |
|-------|--------|
| 🟢 أخضر | شراء قوي - صعود مؤكد |
| 🔵 أزرق | شراء متوسط - صعود محتمل |
| 🔴 أحمر | بيع قوي - هبوط مؤكد |
| 🟠 برتقالي | بيع متوسط - هبوط محتمل |
| ⏳ أبيض | انتظار - لا فرصة حالياً |

---

## ⚠️ تنبيه

> التداول ينطوي على مخاطر. لا تستثمر أكثر مما تستطيع تحمل خسارته.

---

## 👨‍💻 المطور

**Muhannad Daher**

[![GitHub](https://img.shields.io/badge/GitHub-mmuhacker-black?style=for-the-badge&logo=github)](https://github.com/mmuhacker)

[![Contact Us](https://img.shields.io/badge/Contact_Us-black?style=for-the-badge&logo=gmail&logoColor=red)](mailto:madarik.ai.info@gmail.com)

---
</div>



- بوت التداول الذكي
- البيئة: Termux (Android)
- الإصدار: v1.0

---

<div align="center">


⭐ **إذا أعجبتك الأداة، لا تنسَ النجمة!** ⭐

</div>
