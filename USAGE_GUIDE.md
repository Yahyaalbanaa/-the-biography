# 📘 دليل الاستخدام التفصيلي | Detailed Usage Guide

<div align="center">

![Guide](https://img.shields.io/badge/User-Guide-success?style=for-the-badge)
![Language](https://img.shields.io/badge/Language-AR%20%7C%20EN-blue?style=for-the-badge)

</div>

---

## 🎯 المحتويات | Contents

- [البدء السريع](#quick-start)
- [التحكم في الثيمات](#theme-control)
- [التحكم في اللغات](#language-control)
- [التخصيص المتقدم](#advanced-customization)
- [نصائح وحيل](#tips-and-tricks)
- [حل المشاكل](#troubleshooting)

---

<a name="quick-start"></a>

## 🚀 البدء السريع | Quick Start

### الخطوة 1: فتح الموقع
```bash
# افتح ملف index.html في أي متصفح حديث
# يعمل مباشرة بدون الحاجة لخادم ويب
```

### الخطوة 2: التعرف على الواجهة
1. **شريط التنقل العلوي**: للانتقال بين الأقسام
2. **أزرار التحكم** (أعلى اليمين/اليسار):
   - 🌙/☀️ زر الثيم
   - EN/ع زر اللغة

### الخطوة 3: التجربة
- انقر على أزرار التحكم لتجربة الثيمات واللغات
- استكشف الأقسام المختلفة
- جرب التأثيرات التفاعلية

---

<a name="theme-control"></a>

## 🌓 التحكم في الثيمات | Theme Control

### الطرق المتاحة للتبديل:

#### 1️⃣ باستخدام الزر العائم
```
انقر على زر القمر 🌙 للتبديل إلى الثيم الداكن
انقر على زر الشمس ☀️ للتبديل إلى الثيم الفاتح
```

#### 2️⃣ باستخدام لوحة المفاتيح
```
Windows/Linux: Ctrl + Shift + T
Mac: Cmd + Shift + T
```

### خصائص الثيمات:

#### الثيم الفاتح (Light Theme)
- ✅ خلفية بيضاء مريحة للعين
- ✅ نصوص داكنة واضحة
- ✅ مناسب للاستخدام النهاري
- ✅ يوفر طاقة أقل على الشاشات LCD

#### الثيم الداكن (Dark Theme)
- ✅ خلفية داكنة أنيقة
- ✅ نصوص فاتحة واضحة
- ✅ مناسب للاستخدام الليلي
- ✅ يقلل إجهاد العين في الإضاءة المنخفضة
- ✅ يوفر طاقة البطارية على شاشات OLED

### الحفظ التلقائي:
- تُحفظ تفضيلاتك تلقائياً في المتصفح
- يتم استرجاع الثيم المفضل عند العودة للموقع
- يعمل على مستوى الجهاز (لكل متصفح منفصل)

---

<a name="language-control"></a>

## 🌍 التحكم في اللغات | Language Control

### الطرق المتاحة للتبديل:

#### 1️⃣ باستخدام زر اللغة
```
انقر على زر "EN" للتبديل إلى الإنجليزية
انقر على زر "ع" للتبديل إلى العربية
```

#### 2️⃣ باستخدام لوحة المفاتيح
```
Windows/Linux: Ctrl + Shift + L
Mac: Cmd + Shift + L
```

### ما يحدث عند التبديل:

#### التبديل إلى العربية (RTL)
- 🔄 اتجاه الصفحة من اليمين لليسار
- 🔄 الخطوط: Cairo (محسّن للعربية)
- 🔄 جميع النصوص بالعربية
- 🔄 القوائم والعناصر معكوسة

#### التبديل إلى الإنجليزية (LTR)
- 🔄 اتجاه الصفحة من اليسار لليمين
- 🔄 الخطوط: Roboto (محسّن للإنجليزية)
- 🔄 جميع النصوص بالإنجليزية
- 🔄 القوائم والعناصر في الاتجاه الطبيعي

### عناصر مترجمة:
- ✅ قائمة التنقل
- ✅ العناوين الرئيسية
- ✅ جميع النصوص والفقرات
- ✅ أسماء المشاريع والخدمات
- ✅ نموذج الاتصال
- ✅ التذييل

---

<a name="advanced-customization"></a>

## 🎨 التخصيص المتقدم | Advanced Customization

### 1. تغيير الألوان

افتح `css/style.css` وابحث عن CSS Variables:

```css
:root {
    /* الألوان الأساسية - Light Theme */
    --accent-primary: #0066ff;      /* اللون الرئيسي */
    --accent-secondary: #0052cc;    /* اللون الثانوي */
    
    /* يمكنك تغيير أي لون هنا */
    --text-primary: #1a1a1a;
    --bg-primary: #ffffff;
}

[data-theme="dark"] {
    /* الألوان الأساسية - Dark Theme */
    --accent-primary: #3b8efd;
    --accent-secondary: #2f73c9;
    
    /* قم بتخصيص ألوان الثيم الداكن هنا */
}
```

### 2. تعديل التدرجات اللونية

```css
:root {
    --gradient-1: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    --gradient-2: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
    --gradient-3: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
    --gradient-4: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
    
    /* أضف تدرجاتك الخاصة */
    --gradient-custom: linear-gradient(135deg, #ff0000 0%, #00ff00 100%);
}
```

### 3. تغيير الخطوط

افتح `index.html` وعدّل رابط Google Fonts:

```html
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800&family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
```

ثم عدّل في `css/style.css`:

```css
body {
    font-family: 'Tajawal', 'Cairo', sans-serif;
}
```

### 4. إضافة قسم جديد

```html
<!-- في index.html -->
<section id="new-section" class="new-section">
    <div class="container">
        <div class="section-header">
            <h2 class="section-title" data-ar="عنوان القسم" data-en="Section Title">عنوان القسم</h2>
        </div>
        <div class="section-content">
            <!-- محتوى القسم -->
        </div>
    </div>
</section>
```

```css
/* في css/style.css */
.new-section {
    background: var(--bg-secondary);
    padding: var(--spacing-xl) 0;
}
```

### 5. تخصيص المعلومات الشخصية

افتح `index.html` وعدّل:

```html
<!-- معلومات البطل -->
<h1 class="hero-title" data-ar="اسمك هنا" data-en="Your Name Here">اسمك هنا</h1>
<p class="hero-subtitle" data-ar="وظيفتك هنا" data-en="Your Job Here">وظيفتك هنا</p>

<!-- الروابط الاجتماعية -->
<a href="https://github.com/your-username" target="_blank">
    <i class="fab fa-github"></i>
</a>
```

### 6. إضافة لغة ثالثة

افتح `js/script.js` وأضف في كائن translations:

```javascript
const translations = {
    ar: { /* العربية */ },
    en: { /* الإنجليزية */ },
    fr: {
        // الفرنسية (مثال)
        home: 'Accueil',
        about: 'À propos',
        skills: 'Compétences',
        // ... إلخ
    }
};
```

ثم أضف منطق التبديل بين اللغات الثلاث.

---

<a name="tips-and-tricks"></a>

## 💡 نصائح وحيل | Tips & Tricks

### 1. اختصارات لوحة المفاتيح
```
Ctrl/Cmd + Shift + T  →  تبديل الثيم
Ctrl/Cmd + Shift + L  →  تبديل اللغة
Space                 →  التمرير لأسفل
Shift + Space         →  التمرير لأعلى
Home                  →  العودة لبداية الصفحة
End                   →  الذهاب لنهاية الصفحة
```

### 2. التنقل السريع
- انقر على عناصر القائمة للانتقال الفوري
- التمرير سلس وتلقائي
- يتم تمييز القسم النشط تلقائياً

### 3. على الأجهزة المحمولة
- اسحب من اليمين (RTL) أو اليسار (LTR) لفتح القائمة
- انقر خارج القائمة لإغلاقها
- جميع الأزرار مُحسّنة للمس

### 4. التخصيص السريع للألوان
استخدم أدوات المطور في المتصفح:
```javascript
// في console المتصفح
document.documentElement.style.setProperty('--accent-primary', '#ff0000');
```

### 5. تصدير التفضيلات
```javascript
// احفظ تفضيلاتك
const preferences = {
    theme: localStorage.getItem('theme'),
    language: localStorage.getItem('language')
};
console.log(preferences);
```

### 6. تحسين الأداء
- احتفظ بالصور بحجم معقول (< 500KB)
- استخدم WebP للصور عند الإمكان
- فعّل ضغط gzip على الخادم
- استخدم CDN للمكتبات الخارجية

---

<a name="troubleshooting"></a>

## 🔧 حل المشاكل | Troubleshooting

### المشكلة: الثيم لا يتبدل
**الحل:**
1. تأكد من تفعيل JavaScript في المتصفح
2. امسح ذاكرة التخزين المؤقت (Cache)
3. جرب في وضع التصفح الخاص
4. تأكد من عدم وجود أخطاء في Console

```javascript
// اختبر في console
toggleTheme();
```

### المشكلة: اللغة لا تتبدل
**الحل:**
1. تأكد من وجود ملف `js/script.js`
2. تحقق من Console للأخطاء
3. تأكد من وجود السمات data-ar و data-en

```javascript
// اختبر في console
toggleLanguage();
```

### المشكلة: الصور لا تظهر
**الحل:**
1. تحقق من مسارات الصور
2. استخدم صور من مصادر موثوقة (Unsplash, CDN)
3. تأكد من وجود alt text لجميع الصور

```html
<!-- استخدم صور بديلة -->
<img src="https://ui-avatars.com/api/?name=User+Name" alt="User">
```

### المشكلة: القائمة المحمولة لا تعمل
**الحل:**
1. تأكد من وجود class="mobile-menu-toggle"
2. تحقق من تضارب CSS
3. جرب في أجهزة مختلفة

```javascript
// اختبر في console
document.querySelector('.mobile-menu-toggle').click();
```

### المشكلة: التأثيرات لا تعمل
**الحل:**
1. تأكد من دعم المتصفح للـ CSS Variables
2. حدّث المتصفح لآخر إصدار
3. جرب في متصفح آخر

### المشكلة: الخطوط لا تظهر بشكل صحيح
**الحل:**
1. تحقق من اتصال الإنترنت (Google Fonts يحتاج إنترنت)
2. استخدم خطوط محلية كبديل
3. تأكد من تحميل ملفات الخطوط

```html
<!-- خطوط احتياطية -->
<style>
body {
    font-family: 'Cairo', Arial, sans-serif;
}
</style>
```

### المشكلة: بطء تحميل الموقع
**الحل:**
1. قلل حجم الصور
2. استخدم lazy loading للصور
3. قلل من المكتبات الخارجية
4. فعّل ضغط الملفات

```html
<!-- Lazy loading للصور -->
<img src="image.jpg" loading="lazy" alt="Description">
```

### كيفية الإبلاغ عن مشكلة:

1. **افتح Console المتصفح:**
   - Chrome: F12 أو Ctrl+Shift+J
   - Firefox: F12 أو Ctrl+Shift+K
   - Safari: Cmd+Option+C

2. **التقط لقطة شاشة للخطأ**

3. **وصف المشكلة:**
   - ماذا حدث؟
   - ماذا كنت تتوقع؟
   - خطوات إعادة إنتاج المشكلة
   - المتصفح والإصدار
   - نظام التشغيل

---

## 📚 موارد إضافية | Additional Resources

### التعلم والتطوير:
- [MDN Web Docs](https://developer.mozilla.org/) - مرجع شامل لتقنيات الويب
- [CSS Tricks](https://css-tricks.com/) - نصائح وحيل CSS
- [JavaScript.info](https://javascript.info/) - دليل JavaScript الحديث

### أدوات مفيدة:
- [Google PageSpeed Insights](https://pagespeed.web.dev/) - اختبار أداء الموقع
- [Can I Use](https://caniuse.com/) - توافق المتصفحات
- [Color Hunt](https://colorhunt.co/) - لوحات ألوان جاهزة

### مجتمعات وأسئلة:
- [Stack Overflow](https://stackoverflow.com/) - للأسئلة التقنية
- [GitHub Discussions](https://github.com/) - مناقشات المطورين
- [Dev.to](https://dev.to/) - مقالات ونصائح برمجية

---

## 🆘 الدعم | Support

### للحصول على المساعدة:
- 📧 **البريد الإلكتروني**: yahya.albanna@example.com
- 💬 **نموذج الاتصال**: استخدم نموذج الاتصال في الموقع
- 🐙 **GitHub Issues**: افتح issue على المستودع

### أوقات الاستجابة:
- استفسارات عامة: 24-48 ساعة
- مشاكل تقنية: 2-4 أيام
- طلبات ميزات جديدة: حسب الإمكانية

---

<div align="center">

### 🌟 شكراً لاستخدامك الموقع!

**إذا أعجبك المشروع، لا تنسى إعطائه ⭐**

![Thank You](https://img.shields.io/badge/Thank-You-red?style=for-the-badge)

**[⬆ العودة للأعلى | Back to Top](#-دليل-الاستخدام-التفصيلي--detailed-usage-guide)**

</div>