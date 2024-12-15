# CSS Selectors

> [!NOTE]
> CSS selektorlar veb-sahifada HTML elementlariga `style`lar berish uchun ishlatiladi. Selektorlar orqali qaysi elementga style berilishi aniqlanadi.

1. Universal Selector

Universal selektor (`*`) barcha elementlarga style beradi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
</head>
<body>
  <h1>Hello, world!</h1>
  <p>This is an example of the universal selector.</p>
</body>
</html>
```

2. Element (Type) Selector

Element selector ma’lum bir HTML tegiga style beradi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  h1 {
    color: blue;
  }
  p {
    font-size: 18px;
  }
</style>
</head>
<body>
  <h1>This is a style for H1 tags.</h1>
  <p>This is a style for P tags.</p>
</body>
</html>
```

3. Class Selector

Class selektori nuqta (`.`) bilan belgilanadi va bir yoki bir nechta elementga berilishi mumkin.

4. ID Selector

**ID** selektori `#` belgisi bilan chaqiriladi va yagona elementga style beradi.

5. Hierarchy Selectors
   - Child Selector


Faqat bevosita ichki elementlarni tanlaydi.
   

   - Descendant Selector

Ichki barcha elementlarni tanlaydi.

6. Pseudo-classes
   - Hover

Element ustiga kursor qo‘yilganda style beradi.

  - First-child

Birinchi bola elementga style beradi.

7. Pseudo-elements
   - Before

Element oldiga content qo‘shadi.

  - After

Element oxiriga content qo‘shadi.

8. Attribute Selectors
   - Specific Attribute



  - Attribute Starts With