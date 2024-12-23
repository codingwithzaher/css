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
