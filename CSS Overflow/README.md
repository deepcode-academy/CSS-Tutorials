# CSS Overflow

> [!NOTE]
> **overflow** xossasi content o'zining konteyneriga sig'maganida qanday ishlashini belgilaydi. Bu xossa odatda **blok-level** elementlarga nisbatan ishlatiladi va ularga ko'rinishni boshqarish imkonini beradi.

## `overflow` Property Values

1. **visible** (default value):

Content sig'masa, tashqariga chiqib ketadi.

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

