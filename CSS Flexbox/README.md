# CSS Flexbox

> [!NOTE]
> CSSda **Flexbox** (`Flexible Box Layout`) veb-sahifalardagi elementlarni moslashuvchan va samarali joylashtirish uchun ishlatiladi. Flexbox yordamida elementlarni gorizontal yoki vertikal yoʻnalishda joylashtirish, oʻlchamini avtomatik oʻzgartirish va ular orasidagi boʻshliqni boshqarish osonlashadi.

## Enabling Flexbox

Flexbox faqat **flex container**da ishlaydi. Bu uchun konteynerga `display: flex;` xususiyatini qoʻshamiz:

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

## Basic Concepts

Flexbox ikkita asosiy komponentdan iborat:

1. Flex Container: Flexbox qoʻllaniladigan element (`display: flex;`).
2. Flex Items: Container ichidagi barcha **child** elementlar.

## Flexbox Properties

1. **flex-direction**
    - Elementlarni gorizontal yoki vertikal yoʻnalishda joylashtirish uchun ishlatiladi.
      - **row (default):** Elementlar chapdan oʻngga.
      - **row-reverse:** Elementlar oʻngdan chapga.
      - **column:** Elementlar yuqoridan pastga.
      - **column-reverse:** Elementlar pastdan yuqoriga.

```css
.container {
  display: flex;
  flex-direction: row;
  flex-direction: row-reverse;
  flex-direction: column;
  flex-direction: column-reverse;
}
```

2. **justify-content**
    - Elementlar orasidagi gorizontal boʻshliqni boshqaradi.
      - **flex-start (default):** Chapga hizalanadi.
      - **flex-end:** Oʻngga hizalanadi.
      - **center:** Markazda hizalanadi.
      - **space-between:** Elementlar orasida maksimal boʻshliq.
      - **space-around:** Elementlar orasida va chekkalarda bir xil boʻshliq.

```css
.container {
  display: flex;
  justify-content: center; /* Elementlar markazda */
}
```

3. **align-items**
    - Elementlarni vertikal yoʻnalishda joylashtiradi.
      - **stretch (default):** Boʻsh joyni toʻldiradi.
      - **flex-start:** Yuqoriga hizalanadi.
      - **flex-end:** Pastga hizalanadi.
      - **center:** Markazga hizalanadi.
      - **baseline:** Matnning pastki chizigʻiga mos hizalanadi.

```css
.container {
  display: flex;
  align-items: center; /* Elementlar vertikal markazda */
}
```

4. **align-content**
    - Bir nechta qator boʻlsa, ularning orasidagi boʻsh joylarni boshqaradi.
      - **stretch (default):** Qatorlarni choʻzadi.
      - **flex-start:** Yuqoriga hizalanadi.
      - **flex-end:** Pastga hizalanadi.
      - **center:** Markazga hizalanadi.
      - **space-between:** Qatorlar orasida maksimal boʻshliq.
      - **space-around:** Qatorlar orasida va chekkalarda boʻshliq.

```css
.container {
  display: flex;
  flex-wrap: wrap; /* Qatorlarni ruxsat etamiz */
  align-content: space-around;
}
```

5. **flex-wrap**
    - Elementlarni oʻz-oʻzidan qatorlarga boʻlish uchun ishlatiladi.
      - **nowrap (default):** Bitta qatorga joylashtiradi.
      - **wrap:** Elementlar containerga sig'masa, yangi qatorga oʻtadi.
      - **wrap-reverse:** Qatorlar teskari tartibda.

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

## Properties for Flex Items

1. **flex-grow**
   - Elementning boʻsh joyni qancha egallashini aniqlaydi.

```css
.item {
  flex-grow: 1; /* Har bir element teng joy oladi */
}
```

2. **flex-shrink**
   - Elementning kichrayish darajasini boshqaradi.

```css
.item {
  flex-shrink: 1; /* Element kichrayishga ruxsat etiladi */
}
```

3. **flex-basis**
   - Elementning asosiy oʻlchamini belgilaydi.

```css
.item {
  flex-basis: 100px; /* Har bir element kamida 100px kenglikda bo'ladi */
}
```

4. **align-self**
   - Individual element uchun vertikal hizalashni boshqaradi.

```css
.item {
  align-self: center; /* Faqat bir element markazda */
}
```