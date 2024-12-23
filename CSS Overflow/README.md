# CSS Overflow

> [!NOTE]
> **overflow** xossasi content o'zining konteyneriga sig'maganida qanday ishlashini belgilaydi. Bu xossa odatda **blok-level** elementlarga nisbatan ishlatiladi va ularga ko'rinishni boshqarish imkonini beradi.

## `overflow` Property Values

1. **visible (default value):**

Content sig'masa, containerdan tashqariga chiqib ketadi.

```html
<div>
    Bu matn juda uzun va konteyner sig'imi chegarasidan oshib ketadi.
</div>
```

```css
div{
    width: 200px;
    height: 30px;
    overflow: visible;
    border: 1px solid black;
}
```

2. **hidden:**

Sig'magan kontent ko'rsatilmaydi (kesib tashlanadi).

```html
<div>
    Bu matn juda uzun va konteyner sig'imi chegarasidan oshib ketadi.
</div>
```

```css
div{
    width: 200px; 
    height: 100px; 
    overflow: hidden; 
    border: 1px solid black;
}
```

3. **scroll:**

Har doim **scroll-bar** qo'shadi.

```html
<div>
    Bu matn juda uzun va konteyner sig'imi chegarasidan oshib ketadi.
</div>
```

```css
div{
    width: 200px; 
    height: 100px; 
    overflow: scroll; 
    border: 1px solid black;
}
```

4. **auto:**

Sig'magan content uchun avtomatik **skroll-bar** qo'shadi.

```html
<div>
    Bu matn juda uzun va konteyner sig'imi chegarasidan oshib ketadi.
</div>
```

```css
div{
    width: 200px; 
    height: 100px; 
    overflow: auto; 
    border: 1px solid black;
}
```

## `overflow-x` and `overflow-y` Properties

Agar faqat **gorizontal** yoki **vertikal** yo'nalishda overflowni boshqarish kerak bo'lsa, quyidagi xossalar ishlatiladi:

1. **overflow-x:** Faqat gorizontal overflow.

**Qiymatlari:** `visible`, `hidden`, `scroll`, `auto`.

```html
<div>
    Bu matn gorizontal yo'nalishda skroll-bar qo'shadi, lekin vertikal sig'maydi.
</div>
```

```css
div{
    width: 200px; 
    height: 100px; 
    overflow-x: scroll; 
    overflow-y: hidden; 
    border: 1px solid black;
}
```

2. **overflow-y:** Faqat vertikal overflow.

**Qiymatlari:** `visible`, `hidden`, `scroll`, `auto`.

```html
<div>
    Bu matn vertikal yo'nalishda skroll-bar qo'shadi, lekin gorizontal sig'maydi.
</div>
```

```css
div{
     width: 200px; 
    height: 100px; 
    overflow-y: scroll; 
    overflow-x: hidden; 
    border: 1px solid black;
}
```
