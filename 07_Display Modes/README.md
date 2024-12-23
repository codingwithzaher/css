# 🎨 مفهوم أساليب العرض في CSS (Display Modes)

أساليب العرض في CSS تحدد كيفية ظهور العناصر على الصفحة وكيفية تفاعلها مع العناصر الأخرى. هذه الخاصية تمنحك مرونة كبيرة في تصميم الصفحات بشكل متجاوب ومنظم.

---

## 🟢 أساليب عرض العناصر

### 1. `block`

- **الوصف**: العنصر يحتل عرض الصفحة بالكامل ويبدأ في سطر جديد.
- **الأمثلة**: `<div>`, `<p>`, `<section>`.

#### مثال:

```css
div {
  display: block;
}
```

---

### 2. `inline`

- **الوصف**: العنصر يظهر بجانب العناصر الأخرى في نفس السطر، ويأخذ الحجم اللازم فقط لمحتواه.
- **الأمثلة**: `<span>`, `<a>`, `<strong>`.

#### مثال:

```css
span {
  display: inline;
}
```

---

### 3. `inline-block`

- **الوصف**: يجمع ميزات `block` و`inline`؛ حيث يظهر بجانب العناصر الأخرى، ولكنه يحتفظ بقدرة التحكم في العرض والطول.

#### مثال:

```css
div {
  display: inline-block;
}
```

---

### 4. `flex`

- **الوصف**: يجعل العنصر حاوية مرنة تُستخدم لتنظيم العناصر الفرعية بمرونة.

#### مثال:

```css
div {
  display: flex;
}
```

---

### 5. `grid`

- **الوصف**: يُستخدم لتصميم تخطيطات شبكية متقدمة.

#### مثال:

```css
div {
  display: grid;
}
```

---

### 6. `none`

- **الوصف**: يخفي العنصر تمامًا ويزيله من تدفق الصفحة.

#### مثال:

```css
div {
  display: none;
}
```

---

## 🟢 أساليب إخفاء العناصر

### 1. `display: none;`

- **الوصف**: يخفي العنصر تمامًا، كأنه غير موجود في الصفحة.

#### مثال:

```css
div {
  display: none;
}
```

---

### 2. `visibility: hidden;`

- **الوصف**: يخفي العنصر مع الاحتفاظ بمساحته في الصفحة.

#### مثال:

```css
div {
  visibility: hidden;
}
```

---

## 🟢 خصائص العرض والطول

لتحديد أبعاد العناصر، نستخدم الخصائص التالية:

- **`width`**: عرض العنصر.
- **`height`**: ارتفاع العنصر.
- **`max-width` و `max-height`**: الحد الأقصى للعرض والارتفاع.
- **`min-width` و `min-height`**: الحد الأدنى للعرض والارتفاع.

#### مثال:

```css
div {
  width: 200px;
  height: 100px;
  max-width: 300px;
  min-height: 50px;
}
```

---

## 🟢 الحجم والحدود المائلة (Aspect Ratio)

### الخاصية: `aspect-ratio`

- **الوصف**: تحدد نسبة العرض إلى الارتفاع للعنصر.

#### مثال:

```css
div {
  aspect-ratio: 16 / 9;
}
```

---

## 🟢 حساب الهامش والحدود ضمن الحجم

### الخاصية: `box-sizing`

- **`content-box`**: (الإعداد الافتراضي) لا تشمل الأبعاد الحدود والمسافات الداخلية.
- **`border-box`**: تشمل الحدود والمسافات الداخلية ضمن الأبعاد.

#### مثال:

```css
div {
  box-sizing: border-box;
  width: 100px;
  border: 10px solid black;
  padding: 20px;
}
```

**التأثير**: الحجم النهائي للعنصر يبقى 100px مع تضمين الحدود والمسافات الداخلية.

---

## 🟢 ضبط أحجام العناصر على جميع المتصفحات

### لضمان التوافق:

```css
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

---

## 🟢 مثال شامل

#### الكود:

```css
div {
  display: inline-block;
  width: 150px;
  height: 150px;
  box-sizing: border-box;
  border: 5px solid blue;
  padding: 10px;
  margin: 20px auto;
  background-color: lightblue;
}
```

**التأثير**:

- العنصر يظهر بحجم محدد مع تضمين الحدود والمسافات الداخلية.
- تم توسيطه أفقيًا باستخدام الهامش الخارجي.
