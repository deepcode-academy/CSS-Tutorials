# CSS Flexbox

> [!NOTE]
> CSSda **Flexbox** (`Flexible Box Layout`) veb-sahifalardagi elementlarni moslashuvchan va samarali joylashtirish uchun ishlatiladi. Flexbox yordamida elementlarni gorizontal yoki vertikal yoʻnalishda joylashtirish, oʻlchamini avtomatik oʻzgartirish va ular orasidagi boʻshliqni boshqarish osonlashadi.

## Enabling Flexbox

Flexbox faqat flex containerda ishlaydi. Bu uchun konteynerga `display: flex;` xususiyatini qoʻshamiz:

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  display: flex;
}
.item {
  background-color: lightblue;
  padding: 20px;
  margin: 5px;
  border: 1px solid #ccc;
}
```