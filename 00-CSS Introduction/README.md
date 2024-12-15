# CSS Introduction

> [!NOTE]
> CSS (**Cascading Style Sheets**) – bu veb-sahifalarning ko‘rinishini boshqarish uchun ishlatiladigan texnologiya. CSS yordamida HTML elementlariga **style** berish mumkin. CSS orqali veb-sahifalarni zamonaviy va chiroyli ko‘rinishda yaratish mumkin.

## What does CSS do?

1. Design Control: HTML elementlarga **style**lar qo‘shadi (masalan, matn rangini yoki shrift hajmini o‘zgartirish).
2. Separation: HTML strukturasini va **style**ni ajratadi. Bu dasturlarni tartibli va boshqaruvni osonlashtiradi.
3. Reusability: Bir nechta sahifalarda bir xil dizaynni ishlatish imkonini beradi.
4. Responsive Design: urli qurilmalar (telefon, planshet, kompyuter) uchun moslashuvchan dizayn yaratadi.

## How is CSS used?

CSS **3** ta asosiy usulda ishlatiladi:

1. **Inline CSS:** HTML elementning ichida yoziladi.

```html
<p style="color: blue; font-size: 20px;">Bu matn ko‘k rangda va 20px kattalikda.</p>
```

2. **Internal CSS:** HTML hujjatning `<head>` bo‘limida yoziladi va `<style>` tegi ichida bo‘ladi.

```html
<style>
    p {
        color: red;
        font-size: 18px;
    }
</style>
```

3. **External CSS:** Alohida `.css` faylda yoziladi va HTML hujjatga `<link>` orqali ulanadi.

```html
<!-- HTML -->
<link rel="stylesheet" href="styles.css">
```
`styles.css` **faylida:**
```css
p {
    color: green;
    font-size: 16px;
}
```

## CSS Syntax

CSS sintaksisi quyidagi tarkibiy qismlardan iborat:

```css
selector {
    property: value;
}
```
- Selector – qaysi HTML elementga style qo‘llanilishini belgilaydi (masalan, p, h1, .class, #id).
- Property – o‘zgartiriladigan xususiyatni bildiradi (masalan, color, font-size, margin).
- Value – xususiyatga beriladigan qiymat (masalan, blue, 16px, 10px).