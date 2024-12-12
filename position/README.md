# Position

> [!NOTE]
> CSS position xossasi elementning hujjatdagi joylashuvini aniqlash uchun ishlatiladi. Ushbu xossa elementlarni HTML sahifada turli usullarda joylashtirishga yordam beradi.

## position qiymatlari

1. **static** (default qiymat)
    - Element oddiy oqimda (normal flow) joylashadi.
    - Hech qanday maxsus joylashuv ko'rsatmalari (top, right, bottom, left) ishlamaydi.

```css
div {
    position: static;
}
```

2. **relative**
    - Element oddiy oqimda joylashadi, lekin joylashuvini **top**, **right**, **bottom**, **left** xossalari orqali siljitish mumkin.
    - Siljitilganda, elementning asosiy joylashuvi bo'sh qoladi.

```css
div {
    position: relative;
    top: 20px; /* Pastga 20px siljitiladi */
    left: 10px; /* Chapga 10px siljitiladi */
}
```

3. **absolute**
    - Element oddiy oqimdan chiqariladi. U eng yaqin joylashgan **relative**, **absolute**, yoki **fixed** joylashuvga ega ota elementga nisbatan joylashadi.
    - Agar bunday ota element bo'lmasa, u butun sahifa (html element)ga nisbatan joylashadi.

```css
div {
    position: absolute;
    top: 50px;
    left: 30px;
}
```

4. **fixed**
    - Element ekran (viewport)ga nisbatan joylashadi va sahifani skroll qilsangiz ham joyini o'zgartirmaydi.
    - Ko'pincha navigatsiya paneli yoki "Yuqoriga qaytish" tugmalari uchun ishlatiladi.

```css
div {
    position: fixed;
    bottom: 10px; /* Ekranning pastidan 10px */
    right: 10px; /* Ekranning o'ng tomonidan 10px */
}
```

5. **sticky** (CSS3 qiymati)
    - Element oddiy oqimda joylashadi, lekin berilgan joyga (scroll chegarasiga) yetganda ekranda "yopishib" turadi.
    - **top**, **right**, **bottom**, yoki **left** bilan chegarani belgilashingiz kerak.

```css
div {
    position: sticky;
    top: 0; /* Element yuqoridan yopishib turadi */
}
```

## Qo'shimcha xossalar
- **z-index:** Elementlarning qavatini belgilaydi (bir-birining ustidan chiqish tartibi).

```css
div {
    position: absolute;
    z-index: 10; /* Yuqori qavat */
}
```

- **top, right, bottom, left:** Elementning joylashuvini aniqlash uchun ishlatiladi.

```css
div {
    position: absolute;
    top: 20px; /* Element yuqoridan 20px masofada */
    left: 50px; /* Element chapdan 50px masofada */
}
```

