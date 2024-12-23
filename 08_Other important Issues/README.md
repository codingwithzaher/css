# 🎨 لننهي سلسلة CSS بلمحة عن بعض النقاط المهمة!

---

## 💡 الحدود الخارجية (Outline)

- **الوصف**: تحدد الحدود الخارجية التي تحيط بالعناصر خارج الحدود العادية، دون التأثير على حجم العنصر.

#### مثال:

```css
div {
  outline: 2px solid red;
  outline-offset: 5px;
}
```

---

## 💡 النصوص (Texts)

- **خصائص التحكم في النصوص**:
  - **`color`**: تغيير اللون.
  - **`text-align`**: محاذاة النصوص.
  - **`text-transform`**: تغيير حالة الأحرف.

#### مثال:

```css
p {
  color: blue;
  text-align: center;
  text-transform: uppercase;
}
```

---

## 💡 الخطوط (Fonts)

- **خصائص التحكم في الخطوط**:
  - **`font-family`**: نوع الخط.
  - **`font-size`**: حجم الخط.
  - **`font-weight`**: سماكة الخط.

#### مثال:

```css
p {
  font-family: Arial, sans-serif;
  font-size: 16px;
  font-weight: bold;
}
```

---

## 💡 تأثيرات الظل (Shadows)

- **`text-shadow`**: لتطبيق ظل على النصوص.
- **`box-shadow`**: لتطبيق ظل على العناصر.

#### أمثلة:

```css
h1 {
  text-shadow: 2px 2px 5px gray;
}

div {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
```

---

## 💡 الروابط (Links)

- **تخصيص الروابط** باستخدام تأثير التمرير.

#### مثال:

```css
a {
  text-decoration: none;
  color: blue;
}

a:hover {
  color: red;
}
```

---

## 💡 المحتوى الفائض (Overflow)

- **`overflow`**: لإدارة المحتوى الزائد داخل العنصر.

#### مثال:

```css
div {
  width: 100px;
  height: 100px;
  overflow: scroll;
}
```

---

## 💡 تدفق العناصر (Float)

- **`float`**: لتحديد تدفق العناصر داخل الصفحة.

#### مثال:

```css
img {
  float: left;
  margin-right: 10px;
}
```

---

## 💡 قوائم التعداد (Lists)

- **إزالة النقاط** من القوائم.

#### مثال:

```css
ul {
  list-style-type: none;
}
li {
  margin: 5px 0;
}
```

---

## 💡 الجداول (Tables)

- **تصميم الجداول** باستخدام الحدود والمسافات الداخلية.

#### مثال:

```css
table {
  border-collapse: collapse;
  width: 100%;
}

td,
th {
  border: 1px solid black;
  padding: 10px;
}
```

---

## 💡 مواقع العناصر (Position)

- **`position`**: تحديد موقع العنصر بالنسبة للمستند أو العناصر الأخرى.

#### مثال:

```css
div {
  position: absolute;
  top: 50px;
  left: 20px;
}
```

---

## 💡 قوائم الروابط (Navbar)

- **تصميم شريط التنقل** باستخدام `flex`.

#### مثال:

```css
nav ul {
  list-style: none;
  display: flex;
}

nav li {
  margin-right: 15px;
}
```

---

## 💡 القوائم المنسدلة (Dropdowns)

- **إنشاء قوائم منسدلة**.

#### مثال:

```css
.dropdown-content {
  display: none;
  position: absolute;
}

.dropdown:hover .dropdown-content {
  display: block;
}
```

---

## 💡 بداية ونهاية العنصر

- **`:before` و `:after`**: لإضافة محتوى قبل أو بعد العنصر.

#### مثال:

```css
p:before {
  content: ">> ";
}
p:after {
  content: " <<";
}
```

---

## 💡 العدادات (Counters)

- **إضافة عدادات تلقائية** للعناصر.

#### مثال:

```css
ol {
  counter-reset: list-counter;
}

li {
  counter-increment: list-counter;
}

li::before {
  content: counter(list-counter) ". ";
}
```

---

## 💡 الصور المقتطعة (Image Sprites)

- **استخدام صورة واحدة لعدة أيقونات**.

#### مثال:

```css
.icon {
  background: url("sprites.png") no-repeat;
  width: 50px;
  height: 50px;
}

.icon-home {
  background-position: 0 0;
}
```

---

## 💡 عناصر النماذج (Forms)

- **تصميم الحقول والأزرار**.

#### مثال:

```css
input,
textarea {
  padding: 10px;
  border: 1px solid #ccc;
}

button {
  background-color: blue;
  color: white;
  padding: 10px 20px;
}
```

---

## 💡 أولوية التحديد (Specificity)

- **الأولوية في CSS**:
  - الأقل: العنصر (مثل: `p`).
  - الأعلى: المعرّف `id` (مثل: `#myId`).

#### مثال:

```css
p {
  color: red;
}
#myId {
  color: blue;
} /* اللون الأزرق له الأولوية */
```
