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

```html
<!DOCTYPE html>
<html>
<head>
<style>
  .red {
    color: red;
  }
  .large {
    font-size: 24px;
  }
</style>
</head>
<body>
  <p class="red">This is red text.</p>
  <p class="large">This is large text.</p>
  <p class="red large">This is red and large text.</p>
</body>
</html>
```

4. ID Selector

**ID** selektori `#` belgisi bilan chaqiriladi va yagona elementga style beradi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  #special {
    background-color: yellow;
    padding: 10px;
  }
</style>
</head>
<body>
  <p id="special">This is an example of the ID selector.</p>
</body>
</html>
```

5. Hierarchy Selectors
   - Child Selector

Faqat bevosita ichki elementlarni tanlaydi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  div > p {
    color: green;
  }
</style>
</head>
<body>
  <div>
    <p>This is a direct child selector.</p>
    <div>
      <p>This is a nested element. It will not be styled.</p>
    </div>
  </div>
</body>
</html>
```
   

   - Descendant Selector

Ichki barcha elementlarni tanlaydi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  div p {
    font-style: italic;
  }
</style>
</head>
<body>
  <div>
    <p>This styles all nested elements.</p>
    <div>
      <p>This is also selected by the descendant selector.</p>
    </div>
  </div>
</body>
</html>
```

6. Pseudo-classes
   - Hover

Element ustiga kursor qo‘yilganda style beradi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  a:hover {
    color: red;
  }
</style>
</head>
<body>
  <a href="#">Hover over this link.</a>
</body>
</html>
```

  - First-child

Birinchi bola elementga style beradi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  li:first-child {
    font-weight: bold;
  }
</style>
</head>
<body>
  <ul>
    <li>This is the first item.</li>
    <li>This is the second item.</li>
  </ul>
</body>
</html>
```

7. Pseudo-elements
   - Before

Element oldiga content qo‘shadi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  h1::before {
    content: "🌟 ";
  }
</style>
</head>
<body>
  <h1>Added a star!</h1>
</body>
</html>
```

  - After

Element oxiriga content qo‘shadi.

```html
<!DOCTYPE html>
<html>
<head>
<style>
  h1::after {
    content: " ✔";
  }
</style>
</head>
<body>
  <h1>Completed</h1>
</body>
</html>
```

8. Attribute Selectors
   - Specific Attribute

```html
<!DOCTYPE html>
<html>
<head>
<style>
  input[type="text"] {
    border: 2px solid blue;
  }
</style>
</head>
<body>
  <input type="text" placeholder="Enter text">
  <input type="password" placeholder="Enter password">
</body>
</html>
```


  - Attribute Starts With

```html
<!DOCTYPE html>
<html>
<head>
<style>
  a[href^="https"] {
    color: green;
  }
</style>
</head>
<body>
  <a href="https://example.com">HTTPS link</a>
  <a href="http://example.com">HTTP link</a>
</body>
</html>
```