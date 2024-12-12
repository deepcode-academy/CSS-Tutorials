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

## **overflow-x** and **overflow-y** Properties

