# 🎨 مفهوم الحدود في CSS

الحدود هي الخطوط المحيطة بأي عنصر على الصفحة، وهي تُستخدم لإبراز العناصر بصريًا وتحديدها داخل التصميم. باستخدام CSS، يمكنك تخصيص الحدود من حيث الشكل، السمك، اللون، والزوايا للحصول على تأثيرات جمالية مميزة.

---

## 🟡 تحديد شكل حدود العنصر

### الخاصية: `border-style`

تُحدد نمط الحدود.

#### القيم المتاحة:

- `solid`: خط مستمر.
- `dotted`: نقاط صغيرة.
- `dashed`: خطوط متقطعة.
- `double`: خط مزدوج.
- `groove`: حدود محفورة.
- `ridge`: حدود بارزة.
- `inset`: تأثير داخلي.
- `outset`: تأثير خارجي.
- `none`: بدون حدود.

#### مثال:

```css
div {
  border-style: solid;
}
```

**التأثير**: تظهر الحدود كخط مستمر.

---

## 🟡 تحديد سمك الحدود

### الخاصية: `border-width`

تُحدد سماكة الحدود.

#### القيم:

- `thin`: حدود رفيعة.
- `medium`: حدود متوسطة السماكة (الإعداد الافتراضي).
- `thick`: حدود سميكة.
- قيم مخصصة (مثل `2px`، `0.5rem`).

#### مثال:

```css
div {
  border-width: 5px;
}
```

**التأثير**: حدود بسماكة 5 بكسل.

---

## 🟡 تحديد لون الحدود

### الخاصية: `border-color`

تُحدد لون الحدود باستخدام طرق الألوان المختلفة مثل:

- الكلمات المفتاحية (مثل `red`، `blue`).
- `rgb` أو `rgba` (لشفافية إضافية).
- `hsl` أو `hsla`.
- النظام الست عشري (`#`).

#### مثال:

```css
div {
  border-color: red;
}
```

**التأثير**: تظهر الحدود بلون أحمر.

---

## 🟡 تحديد الحدود لكل جهة على حدة

### الخاصيات:

- `border-top`
- `border-right`
- `border-bottom`
- `border-left`

#### مثال:

```css
div {
  border-top: 3px solid blue; /* الحدود العلوية */
  border-right: 5px dashed green; /* الحدود اليمنى */
  border-bottom: 2px dotted red; /* الحدود السفلية */
  border-left: 4px double black; /* الحدود اليسرى */
}
```

**التأثير**: تظهر الحدود بألوان وأشكال مختلفة حسب الجهة.

---

## 🟡 تعريف كل خصائص الحدود في سطر واحد

### الخاصية: `border`

تجمع بين السمك، الشكل، واللون.

#### الصيغة:

```css
border: [width] [style] [color];
```

#### مثال:

```css
div {
  border: 2px dashed orange;
}
```

**التأثير**: حدود برتقالية اللون، متقطعة، وسماكتها 2 بكسل.

---

## 🟡 تحديد شكل زوايا الحدود

### الخاصية: `border-radius`

تُستخدم لجعل زوايا العنصر دائرية أو مستديرة.

#### القيم:

- وحدات ثابتة (مثل `10px`، `50px`).
- نسب مئوية (`50%` لتحويل العنصر إلى شكل دائري إذا كان مربعًا).

#### مثال:

```css
div {
  border: 2px solid black;
  border-radius: 10px;
}
```

**التأثير**: تظهر زوايا العنصر مستديرة بمقدار 10 بكسل.

#### مثال لشكل دائري كامل:

```css
div {
  border: 3px solid purple;
  border-radius: 50%; /* يجعل العنصر دائريًا إذا كان مربعًا */
}
```

**التأثير**: يتحول العنصر إلى شكل دائري.

---

## 🟡 مثال شامل لتخصيص الحدود

### كود:

```css
div {
  border: 4px solid blue; /* حدود عامة */
  border-top: 2px dashed red; /* حدود علوية خاصة */
  border-radius: 15px; /* زوايا مستديرة */
}
```

**التأثير**:

- حدود زرقاء سميكة عامة.
- حد علوي أحمر متقطع.
- زوايا مستديرة بمقدار 15 بكسل.

---

## 🪄 الخلاصة

- استخدم `border-style` لتحديد شكل الحدود.
- حدد سماكتها باستخدام `border-width`.
- أضف ألوانًا باستخدام `border-color`.
- خصص الحدود لكل جهة على حدة أو اجمع كل الخصائص معًا باستخدام `border`.
- للحصول على زوايا دائرية، استخدم `border-radius`.

باستخدام هذه الخصائص، يمكنك تصميم حدود احترافية لإبراز العناصر وإضافة لمسات جمالية إلى صفحات الويب!
