# CSS Float

> [!NOTE]
> CSSda float elementi boshqa elementlarni o'ngga yoki chapga surish uchun ishlatiladi. Ushbu usul veb-sahifa dizaynida, ayniqsa matn va rasmni yonma-yon joylashtirishda foydali bo'lishi mumkin. 

1. Basic Values of `float`

- **float**ning quyidagi qiymatlari bor:
  - **left:** Elementni chapga suradi.
  - **right:** Elementni o'ngga suradi.
  - **none:** Element surilmaydi (bu standart qiymat).
  - **inherit:** Element **float** qiymatini ota elementdan meros qilib oladi.

2. `float` bilan ishlashning umumiy tartibi

Siz **float** ishlatganda, surilishi kerak bo'lgan elementlar keyingi kontent oqimidan chiqadi, ya'ni ular boshqa elementlar ustiga chiqib ketishi yoki joylashuvga ta'sir qilishi mumkin.

**Misol:** Matn va rasmni yonma-yon joylashtirish

```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Float misol</title>
</head>
<body>
    <img src="https://via.placeholder.com/200" alt="Rasm" class="rasm">
    <div class="matn">
        <p>
            Bu matn suzuvchi rasmning o'ng tomonida joylashadi. 
            `float: left` xususiyati orqali rasm chap tomonga joylashadi, 
            qolgan matn esa uning yonidan oqib keladi. Ushbu usul veb-dizaynda 
            tez-tez ishlatiladi.
        </p>
    </div>
</body>
</html>
```

```css
.rasm {
    float: left;
    width: 200px;
    margin-right: 15px;
}
.matn {
    font-size: 16px;
    line-height: 1.6;
}
```

3. **clear:**

Agar bir nechta elementlarni suradigan bo'lsangiz va keyingi elementlar surilganlardan keyin joylashishini xohlasangiz, **clear** xususiyatidan foydalaning.

```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clear misol</title>
</head>
<body>
    <img src="https://via.placeholder.com/200" alt="Rasm" class="rasm">
    <div class="matn">
        <p>
            Bu matn suzuvchi rasmning o'ng tomonida joylashadi. 
        </p>
    </div>
    <div class="footer">
        Bu footer, va u suzuvchi elementlardan keyin joylashadi.
    </div>
</body>
</html>
```

```css
.rasm {
    float: left;
    width: 200px;
    margin-right: 15px;
}
.matn {
    font-size: 16px;
    line-height: 1.6;
}
.footer {
    clear: both;
    background-color: #f0f0f0;
    padding: 10px;
    text-align: center;
}
```

