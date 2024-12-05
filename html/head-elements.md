<div dir="rtl" style="text-align: right;">

# `<head>`

يحتوي `<head>` على معلومات وصفية حول المستند، أغلبها لا يتم عرضها مباشرةً في المتفصح لكنها تساعد المتصفح ومحركات البحث في فهم محتوى الصفحة بشكل أفضل.

**مثال:**

</div>

```html
<head>
  <title>عنوان الصفحة</title>
  <meta charset="UTF-8">
</head>
```

<div dir="rtl" style="text-align: right;">

_لا توجد خصائص (Attributes) مخصصة للعنصر `<head>`, ولكن يحتوي على عدة عناصر هامة مثل `<title>` و `<meta>`._

---

**العناصر الأساسية في `<head>`**

## `<title>`
يحدد عنوان الصفحة الذي يظهر في شريط العنوان أو في التبويب في المتصفح. يحدد موضوع الصفحة.

**مثال:**

</div>

```html
<title>عنوان الصفحة</title>
```

<div dir="rtl" style="text-align: right;">

_لا توجد خصائص (Attributes) مخصصة لوسم `<title>`._

## `<meta>`
تستخدم لإضافة معلومات وصفية (metadata) حول الصفحة، وتكون ذات أهمية خاصة لمحركات البحث والمتصفحات.

**أمثلة على أنواع عناصر `<meta>` الشائعة:**

1. **تحديد ترميز الصفحة (Encoding):**
   يساعد في التأكد من أن جميع الأحرف يتم عرضها بشكل صحيح في المتصفح.
   
</div>

   ```html
   <meta charset="UTF-8">
   ```

<div dir="rtl" style="text-align: right;">

2. **التوافق مع الأجهزة المختلفة:**
   لضبط عرض الصفحة لتكون متجاوبة مع شاشات الهواتف والأجهزة المختلفة.
   
</div>

   ```html
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   ```

<div dir="rtl" style="text-align: right;">

   - شرح content="width=device-width": يُظهر الصفحة حسب عرض الجهاز نفسه، بدلاً من أن تظهر الصفحة على عرض شاشة الديسكتوب.

   - initial-scale=1.0": يتحكم في عرض الصفحة عند فتحها، **1.0** يعني أن عرض الصفحة سيكون كما هو بدون تكبير أو تصغير. مثلاً إذا كانت القيمة **1.2** ستظهر الصفحة أكبر من العرض الطبيعي.

   - يُفضّل أيضاً تحديد أكبر قيمة للتصغير والتكبير باستخدام `minimum-scale` و `maximum-scale`. مثلاً:

</div>

        ```html
        <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0, maximum-scale=5.0" />
        ```

<div dir="rtl" style="text-align: right;">

1. **وصف الصفحة لمحركات البحث:**

</div>

   ```html
   <meta name="description" content="دليل حول وسوم HTML الأساسية.">
   ```

<div dir="rtl" style="text-align: right;">

1. **الكلمات المفتاحية (Keywords):**
   تستخدم لإضافة كلمات مفتاحية تساعد محركات البحث على فهم محتوى الصفحة، وإظهارها ضمن نتائج البحث ذات صلة.
   
</div>

   ```html
   <meta name="keywords" content="HTML, تعلم HTML, تطوير ويب">
   ```

<div dir="rtl" style="text-align: right;">

5. **تحديد صاحب الصفحة أو كاتب المحتوى:**

</div>

   ```html
   <meta name="author" content="اسم الكاتب">
   ```