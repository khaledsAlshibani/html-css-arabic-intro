<div dir="rtl">

<h1>وسوم HTML</h1>

## الوسوم الأساسية

### وسم `<html>`
الوسم الأساسي حيث يمثل ال root في صفحات الويب (root of an HTML document) الذي يحتوي على كل محتويات HTML في صفحة الويب.

**مثال:**
```html
<html lang="ar">
    <head><!-- head elements --></head>
    <body><!-- Body elements --></body>
</html>
```

**بعض attributes تخص الوسم**:
| المصطلح            | الوصف                                                                                       |
|--------------------|---------------------------------------------------------------------------------------------|
| <code dir="ltr">lang</code>  | لتحديد اللغة. ويفضّل دائماً أن يتم استخدامه.              |
| <code dir="ltr">dir</code>   | لتحديد اتجاه النص (مثل `rtl` للعربية و`ltr` للُغات الأخرى).               |

---

### وسم `<head>`
يحتوي على عناصر metadata والعناصر التي لا تظهر مباشرةً في المحتوى، مثل العنوان الذي يظهر في تبويبة المتصفح.

**مثال:**
```html
<head>
  <title>عنوان لصفحة ويب</title>
</head>
```

_لا يوجد attributes تستخدم لوسم ال head_

---

### وسم `<body>`
يحتوي على كل العناصر التي تُعرض في صفحة الويب.

**مثال:**
```html
<body>
    <!-- body elements -->
</body>
```

**بعض attributes تخص الوسم**:
لا يوجد attrs خاصة لهذا الوسم، ولكن من الممكن استخدام ال global attributes.

---

## عناصر ال `<head>`

### وسم `<title>`
يعرض عنوان الصفحة في شريط العنوان أو التبويب في المتصفح.

**مثال:**
```html
<title>عنوان لصفحة HTML</title>
```

_لا يوجد attributes تستخدم للوسم `head`_

---

### وسم `<meta>`
لتحديد بيانات عن الصفحة.

**أمثلة على أهم أنواع ال `<meta>`:**

1. **تحديد ترميز الصفحة:**
```html
<meta charset="UTF-8">
```

2. **وصف الصفحة لمحركات البحث**
```html
<meta name="description" content="مثال على صفحة HTML تحتوي على أهم وسوم الميتا.">
```

3. **كلمات مفتاحية للصفحة، تُستخدم لمحركات البحث**
```html
<meta name="keywords" content="HTML, CSS, تعلم البرمجة, تطوير الويب">
```

4. **لتحديد كاتب أو مالك المحتوى**
```html
<meta name="author" content="اسم الكاتب أو الشركة">
```

5. **تحديد عرض الصفحة لتكون متجاوبة مع الأجهزة المختلفة**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

## عناصر ال `<body>`

### وسم `<header>`
وسم دلالي عادة يستخدم في رأس الصفحة، حيث يكون الجزء الأعلى الذي يظهر في صفحات الويب، عادة يحتوي على عنوان الموقع وصورة أو شعار.

**مثال:**
```html
<header>
  <h1>عنوان الموقع</h1>
</header>
```

---

### وسم `<footer>`
يمثل تذييل الصفحة (الجزء الذي يوجد أسفل الصفحة) يحتوي عادةً على معلومات حقوق النشر.

**مثال:**
```html
<footer>
  <p>&copy; 2023</p>
</footer>
```

---

### وسم `<article>`
يستخدم ك container لمحتوى مستقل، مثل مقالات المدونات أو الأخبار.

**مثال:**
```html
<article>
  <h2>عنوان المقال</h2>
  <p>بعض الوصف</p>
</article>
```

---

### وسم `<aside>`
يُستخدم كعنصر جانبي يظهر على إحدى جوانب الصفحات.

---

### وسم `<p>`
يستخدم لكتابة الفقرات النصية.

**مثال:**
```html
<p>هذا هو نص الفقرة.</p>
```

---

### وسم `<h1> - <h6>`
وسوم العناوين من H1 إلى H6، حيث H1 هو الأكثر أهمية وH6 الأقل.
ولا يستخدم `<h1>` سوى مرة وحدة في نفس الصفحة، ويُفضل أن تحتوي كل صفحة على العنصر.

**مثال:**
```html
<h1>العنوان الرئيسي</h1>
<h2>العنوان الثانوي</h2>
```

---

### وسم `<del>`
اختصار لـ deleted، يُستخدم للنص المحذوف أو المشطوب. ويستخدم غالباً مع العنصر `<ins>`.

---

### وسم `<ins>`
اختصار ل inserted، يستخدم لنص تم إضافته، وغالباً يرتبط استخدامه بالعنصر `<del>`

**مثال:**
(_مأخوذ من MDN Web Docs_)
```html
<p>“You're late!”</p>
<del>
  <p>“I apologize for the delay.”</p>
</del>
<ins cite="../howtobeawizard.html" datetime="2018-05">
  <p>“A wizard is never late …”</p>
</ins>
```

**بعض attributes تخص الوسم**:
| المصطلح            | الوصف                                                                                       |
|--------------------|---------------------------------------------------------------------------------------------|
| <code dir="ltr">cite</code>  | يستقبل رابط يوضح الإضافة            |
| <code dir="ltr">datetime</code>   | التاريخ والوقت الذي تمت فيه الإضافة مثل <code dir="ltr">datetime="2018-05"</code>              |

---

### وسم `<mark>`
يُستخدم لتسليط الضوء على جزء من نَص (hilight text).

**مثال:**
```html
<p>بعض الكلمات من النص ولكن هذا <mark>نص مميز</mark> ليس كهذا النص.</p>
```

---

### وسم `<i>`
اختصار لـ italic ويُظهر النص بتنسيق مائل، ولكن بفضّل تنسيق النصوص باستخدام css بدلاً من استخدام العنصر.

**مثال:**
```html
<i>نص مائل</i>
```

### وسم `<b>`
اختصار لـ bold، ويستخدم لعرض النص بحيث يكون غامق.

**مثال:**
```html
<b>نص بولد</b>
```

---

### وسم `<u>`
اختصار ل underlined، يستخدم لوضع خط أسفل النص.

**مثال:**
```html
<u>نص أسفله خط</u>
```

---

### وسم `<big>`
يتحكم بحجم النص ويقوم بتكبير الحجم.

> ⚠️ هذا الوسم deprecated، يفضّل تجنب استخدامه.

**مثال:**
```html
<big>نص كبير.</big>
```

---

### وسم `<small>`
يتحكم بحجم النص ويقوم بتصغير الحجم.

**مثال:**
```html
<small>نص صغير.</small>
```

---

### وسم `<sup>`
يستخدم للنص المرتفع قليلاً عن باقي النص، مثلاً يستخدم للقوى (الأسس).

**مثال:**
```html
X = Y<sup>2</sup>
```

---

### وسم `<sub>`
عكس العنصر `<sup>` حيث يستخدم للنص المنخفض مثل العدد الذري للعناصر الكيميائية.

**مثال:**
```html
H<sub>2</sub>O
```

---

### وسم `<strong>`
يستخدم لتحديد نص ذو أهمية، وهذا العنصر له معنى دلالي (semantic meaning) ويعني strong emphasis. ويختلف عن العنصر `<b>`، حيث أن العنصر `<b>` يستخدم فقط لغرض التنسيق وليس له معنى دلالي. لهذا لا يُفضل استخدام العنصر `<strong>` فقط من أجل تنسيق كنص بولد.

**مثال:**
```html
<strong>نص مهم</strong>
```

---

### وسم `<br>`
اختصار لـ line break. ويستخدم لبداية سطر جديد.

**مثال:**
```html
<p>سطر أول<br>سطر ثاني</p>
```

_لا يوجد attributes تستخدم لوسم ال head_

---

### وسم `<em>`
اختصار لـ Emphasis. هذا العنصر يختلف عن العنصر `<i>` بأن له معنى دلالي لهذا لا يتم استخدامه فقط من أجل تنسيق كنص مائل.
تماماً كما يوجد فرق بين العنصرين `<strong>` و `<b>`.

**مثال:**
```html
<p>هذا العنصر <em>ليس</em> للتنسيق</p>
```

---

### وسم `<pre>`
اختصار لـ Preformatted. ويُستخدم لإظهار النص كما هو، غالباً يستخدم لإظهار الكود (code snippets).

**مثال:**
سيتم طباعة الشكل كما هو تماماً دون حذف أي مسافة أو سطر.
```html
<pre>
    ^__^
    (oo)\_______
    (__)\       \\/\
        ||----w |
        ||     ||
</pre>
```

---

### وسم `<code>`
يعرض النص على أنه كود برمجي. ويستخدم لل inline code. وليس كما pre لل code blocks.

```html
لطباعة نص في الجافاسكريبت تستخدم: <code>console.log("some text to print")</code>
```

---

- samp
- hr
- blockquote
- q
- abbr