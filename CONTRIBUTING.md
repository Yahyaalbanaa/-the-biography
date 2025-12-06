# 🤝 دليل المساهمة | Contributing Guide

<div align="center">

![Contributing](https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=for-the-badge)
![PRs](https://img.shields.io/badge/PRs-Welcome-blue?style=for-the-badge)

**نرحب بمساهماتكم في تطوير المشروع!**

**We welcome your contributions to improve this project!**

</div>

---

## 📋 المحتويات | Contents

- [كيفية المساهمة](#how-to-contribute)
- [معايير الكود](#code-standards)
- [عملية Pull Request](#pull-request-process)
- [الإبلاغ عن المشاكل](#reporting-issues)
- [اقتراح ميزات جديدة](#suggesting-features)
- [دليل الأسلوب](#style-guide)

---

<a name="how-to-contribute"></a>

## 🚀 كيفية المساهمة | How to Contribute

### الخطوات الأساسية:

#### 1. Fork المستودع
```bash
# انقر على زر Fork في الصفحة الرئيسية للمستودع
```

#### 2. استنساخ المستودع محلياً
```bash
git clone https://github.com/your-username/portfolio.git
cd portfolio
```

#### 3. إنشاء فرع جديد
```bash
# للميزات الجديدة
git checkout -b feature/feature-name

# لإصلاح الأخطاء
git checkout -b fix/bug-description

# للتوثيق
git checkout -b docs/documentation-update
```

#### 4. إجراء التغييرات
- اكتب كود نظيف ومنظم
- اتبع معايير المشروع
- أضف تعليقات واضحة

#### 5. اختبار التغييرات
```bash
# افتح index.html في المتصفح
# تأكد من عمل جميع الميزات
# اختبر على أجهزة مختلفة
```

#### 6. Commit التغييرات
```bash
git add .
git commit -m "وصف واضح للتغييرات"
```

#### 7. Push إلى GitHub
```bash
git push origin feature/feature-name
```

#### 8. فتح Pull Request
- اذهب إلى صفحة المستودع على GitHub
- انقر على "New Pull Request"
- اختر الفرع الخاص بك
- اكتب وصفاً تفصيلياً للتغييرات

---

<a name="code-standards"></a>

## 📐 معايير الكود | Code Standards

### HTML

#### الهيكل:
```html
<!-- ✅ جيد - استخدام semantic HTML -->
<section class="about">
    <div class="container">
        <h2>نبذة عني</h2>
        <p>المحتوى هنا</p>
    </div>
</section>

<!-- ❌ سيء - استخدام div فقط -->
<div class="about">
    <div>
        <div>نبذة عني</div>
        <div>المحتوى هنا</div>
    </div>
</div>
```

#### المعايير:
- ✅ استخدم HTML5 الدلالي (semantic HTML)
- ✅ أضف alt text لجميع الصور
- ✅ استخدم ARIA labels للعناصر التفاعلية
- ✅ تأكد من صحة البنية (validate HTML)
- ✅ استخدم مسافات بادئة 4 spaces

### CSS

#### التنظيم:
```css
/* ✅ جيد - تنظيم واضح */
.section {
    /* Layout */
    display: flex;
    padding: 2rem;
    
    /* Typography */
    font-size: 1rem;
    color: var(--text-primary);
    
    /* Visual */
    background: var(--bg-primary);
    border-radius: 8px;
    
    /* Animation */
    transition: all 0.3s ease;
}

/* ❌ سيء - غير منظم */
.section {
    color: var(--text-primary);
    padding: 2rem;
    transition: all 0.3s ease;
    display: flex;
    background: var(--bg-primary);
    font-size: 1rem;
}
```

#### المعايير:
- ✅ استخدم CSS Variables للألوان
- ✅ اتبع ترتيب الخصائص (Layout → Typography → Visual → Animation)
- ✅ استخدم BEM naming أو semantic classes
- ✅ أضف تعليقات للأقسام الكبيرة
- ✅ تأكد من التجاوب (responsive)
- ✅ استخدم مسافات بادئة 4 spaces

### JavaScript

#### الكود النظيف:
```javascript
// ✅ جيد - وظائف واضحة ومنظمة
function toggleTheme() {
    const currentTheme = getCurrentTheme();
    const newTheme = currentTheme === 'light' ? 'dark' : 'light';
    applyTheme(newTheme);
    saveThemePreference(newTheme);
}

// ❌ سيء - كود غير منظم
function t() {
    let a = document.body.getAttribute('data-theme');
    if(a=='light'){document.body.setAttribute('data-theme','dark')}else{document.body.setAttribute('data-theme','light')}
}
```

#### المعايير:
- ✅ استخدم ES6+ (const, let, arrow functions)
- ✅ أسماء متغيرات ووظائف واضحة
- ✅ أضف تعليقات للكود المعقد
- ✅ تجنب التكرار (DRY principle)
- ✅ استخدم async/await للعمليات غير المتزامنة
- ✅ معالجة الأخطاء (error handling)
- ✅ استخدم مسافات بادئة 4 spaces

---

<a name="pull-request-process"></a>

## 📝 عملية Pull Request | Pull Request Process

### قبل فتح PR:

#### ✅ Checklist:
```
□ اختبرت الكود على متصفحات مختلفة (Chrome, Firefox, Safari)
□ اختبرت على أجهزة مختلفة (Desktop, Tablet, Mobile)
□ الكود يعمل في الثيم الفاتح والداكن
□ الكود يعمل في اللغتين العربية والإنجليزية
□ لا توجد أخطاء في Console
□ الكود متوافق مع معايير المشروع
□ أضفت تعليقات للكود الجديد
□ حدّثت التوثيق إذا لزم الأمر
```

### وصف PR:

#### القالب:
```markdown
## نوع التغيير | Type of Change
- [ ] ميزة جديدة (Feature)
- [ ] إصلاح خطأ (Bug Fix)
- [ ] تحسين (Enhancement)
- [ ] توثيق (Documentation)
- [ ] تنسيق (Styling)

## الوصف | Description
وصف واضح وموجز للتغييرات.

## الدافع والسياق | Motivation and Context
لماذا هذا التغيير ضروري؟ ما المشكلة التي يحلها؟

## كيفية الاختبار | How to Test
خطوات لاختبار التغييرات:
1. ...
2. ...

## لقطات الشاشة | Screenshots
إن وجدت، أضف لقطات شاشة للتغييرات البصرية.

## الأجهزة المختبرة | Tested Devices
- [ ] Desktop
- [ ] Tablet
- [ ] Mobile

## المتصفحات المختبرة | Tested Browsers
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Edge
```

### مراجعة PR:

سيتم مراجعة الـ PR من قبل المسؤولين وقد يُطلب منك:
- إجراء تعديلات
- إضافة اختبارات
- توضيح بعض النقاط

---

<a name="reporting-issues"></a>

## 🐛 الإبلاغ عن المشاكل | Reporting Issues

### قبل فتح Issue:

#### ✅ تحقق من:
1. لم يتم الإبلاغ عن نفس المشكلة سابقاً
2. جربت تحديث المتصفح
3. مسحت ذاكرة التخزين المؤقت
4. جربت في متصفح آخر

### قالب Issue للأخطاء:

```markdown
## وصف المشكلة | Bug Description
وصف واضح ومختصر للمشكلة.

## خطوات إعادة الإنتاج | Steps to Reproduce
1. اذهب إلى '...'
2. انقر على '....'
3. مرر لأسفل إلى '....'
4. شاهد الخطأ

## السلوك المتوقع | Expected Behavior
ما كان يجب أن يحدث.

## السلوك الفعلي | Actual Behavior
ما حدث فعلاً.

## لقطات الشاشة | Screenshots
إن أمكن، أضف لقطات شاشة.

## البيئة | Environment
- **المتصفح**: Chrome 120
- **نظام التشغيل**: Windows 11
- **حجم الشاشة**: 1920x1080
- **اللغة**: العربية
- **الثيم**: الداكن

## معلومات إضافية | Additional Context
أي معلومات أخرى مفيدة.

## رسائل الأخطاء | Error Messages
```
أضف رسائل الأخطاء من Console هنا
```
```

---

<a name="suggesting-features"></a>

## 💡 اقتراح ميزات جديدة | Suggesting Features

### قالب اقتراح الميزات:

```markdown
## عنوان الميزة | Feature Title
اسم واضح للميزة المقترحة.

## الوصف | Description
وصف تفصيلي للميزة وكيف ستعمل.

## الدافع | Motivation
لماذا هذه الميزة مفيدة؟ ما المشكلة التي ستحلها؟

## الاستخدام المقترح | Proposed Usage
```javascript
// مثال على كيفية استخدام الميزة
```

## البدائل | Alternatives
هل فكرت في حلول بديلة؟

## معلومات إضافية | Additional Context
أي معلومات أخرى، لقطات شاشة، أمثلة من مواقع أخرى.
```

---

<a name="style-guide"></a>

## 🎨 دليل الأسلوب | Style Guide

### التسمية | Naming Conventions

#### Classes CSS:
```css
/* استخدم kebab-case */
.hero-section { }
.nav-menu { }
.contact-form { }

/* استخدم BEM للعناصر المركبة */
.card { }
.card__title { }
.card__content { }
.card--featured { }
```

#### Variables JavaScript:
```javascript
// استخدم camelCase للمتغيرات والوظائف
const currentTheme = 'light';
function toggleLanguage() { }

// استخدم PascalCase للـ Classes
class ThemeManager { }

// استخدم UPPER_CASE للثوابت
const MAX_ITEMS = 10;
const API_URL = 'https://api.example.com';
```

### التعليقات | Comments

#### HTML:
```html
<!-- ========================
     Hero Section
     ======================== -->
<section class="hero">
    <!-- Profile Image -->
    <img src="profile.jpg" alt="Profile">
</section>
```

#### CSS:
```css
/* ===========================
   Hero Section Styles
   =========================== */
.hero {
    /* Main styles */
}

/* Responsive breakpoint */
@media (max-width: 768px) {
    /* Mobile styles */
}
```

#### JavaScript:
```javascript
// ===========================
// Theme Management
// ===========================

/**
 * Toggle between light and dark themes
 * @returns {void}
 */
function toggleTheme() {
    // Implementation
}
```

### Commit Messages:

#### التنسيق:
```
نوع: وصف قصير

وصف تفصيلي اختياري

Fixes #issue_number
```

#### الأنواع:
```
feat:     ميزة جديدة
fix:      إصلاح خطأ
docs:     تحديث توثيق
style:    تنسيق الكود
refactor: إعادة هيكلة
perf:     تحسين أداء
test:     إضافة اختبارات
chore:    مهام صيانة
```

#### أمثلة:
```bash
git commit -m "feat: إضافة وضع القراءة الليلية"
git commit -m "fix: إصلاح مشكلة التبديل بين اللغات"
git commit -m "docs: تحديث دليل الاستخدام"
```

---

## 🌟 نصائح للمساهمين | Tips for Contributors

### 1. ابدأ صغيراً
- لا تحاول تغيير كل شيء دفعة واحدة
- ابدأ بإصلاحات بسيطة أو تحسينات صغيرة
- تعرّف على بنية المشروع أولاً

### 2. التواصل
- اسأل قبل العمل على ميزات كبيرة
- شارك أفكارك في Issues
- تفاعل مع المراجعين

### 3. الاختبار
- اختبر على متصفحات مختلفة
- اختبر على أجهزة مختلفة
- تأكد من عدم كسر الميزات الموجودة

### 4. التوثيق
- وثّق الكود الجديد
- حدّث README إذا لزم الأمر
- أضف أمثلة عند الحاجة

### 5. الصبر
- المراجعة قد تستغرق وقتاً
- كن مستعداً للتعديلات
- تقبل النقد البنّاء

---

## 📞 التواصل | Contact

### للأسئلة والمساعدة:
- 📧 **البريد**: yahya.albanna@example.com
- 💬 **GitHub Discussions**: للمناقشات العامة
- 🐛 **GitHub Issues**: للمشاكل التقنية

---

## 🏆 المساهمون | Contributors

شكراً لجميع من ساهم في تطوير المشروع! 🙏

<div align="center">

### 🌟 نقدّر مساهماتكم!

![Thank You](https://img.shields.io/badge/Thank-You-red?style=for-the-badge)

**[⬆ العودة للأعلى | Back to Top](#-دليل-المساهمة--contributing-guide)**

</div>