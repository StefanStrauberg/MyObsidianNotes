### Семантика HTML5

Семантика HTML5 относится к использованию специфических тегов, таких как `<header>`, `<footer>`, `<nav>`, `<article>`, `<section>` и др., для обеспечения более четкой структуры и смысла веб-контента. Это улучшает доступность, SEO и способствует лучшему пониманию как людьми, так и машинами.

### Зачем использовать семантические теги HTML?

Использование семантических тегов улучшает доступность сайта, оптимизирует его для поисковых систем (SEO) и обеспечивает более четкую структуру и смысл контента. Это способствует лучшему пониманию как пользователями, так и машинами, что приводит к улучшению удобства и пользовательского опыта.

### Классификация HTML-тегов:
- **Семантические**
- **Несемантические**

#### Семантические элементы

Семантические элементы имеют значимые названия, которые отражают тип контента. Например: `header`, `footer`, `table` и т. д. HTML5 вводит множество семантических элементов, что делает код более понятным для разработчиков и указывает браузеру, как их обрабатывать.
- `<article>`
- `<aside>`
- `<details>`
- `<figcaption>`
- `<figure>`
- `<footer>`
- `<header>`
- `<main>`
- `<mark>`
- `<nav>`
- `<section>`

### Тег `<article>`

Тег `<article>` содержит независимый контент, который не требует дополнительного контекста, например, запись блога или статья в газете.

**Пример:** Ниже приведен пример использования тега `<article>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Article Tag</title>
    <style>
        h1 {
        Color:#006400;
        font-size:50px;
        Text-align:left;
        }
        p {
        font-size:25px;
        text-align:left;
        margin-top:-40px;
        }
    </style>
</head>

<body>
    <article>
        <h1>GeeksforGeeks</h1>
        <p>A Computer Science Portal for Geeks</p>
    </article>
</body>

</html>
```

### Тег `<aside>`

Тег `<aside>` используется для размещения контента в боковой панели, то есть отдельного от основного контента. Он связан с окружающим содержимым.

**Пример:** Ниже приведен пример использования тега `<aside>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Aside Tag</title>
    <style>
        h4 {
        Color:#006400;
        font-size:50px;
        Text-align:none;
        margin-bottom:0px;
        }
        p {
        font-size:25px;
        text-align:none;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <p>GeeksforGeeks is a Computer Science Portal</p>
    <aside>
        <h4>GeeksForGeeks</h4>
        <p>GeeksforGeeks is a computer Science platform
            where you can learn good programming.
        </p>
    </aside>
</body>

</html>
```

### Теги `<details>` и `<summary>`

Тег `<details>` определяет дополнительные сведения, которые пользователь может скрыть или просмотреть. Тег `<summary>` задает видимый заголовок для элемента `<details>`.

**Пример:** Ниже приведен пример использования тегов `<details>` и `<summary>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Detail and summary Tag</title>
    <style>
        .GFG {
        Color:#006400;
        font-size:50px;
        Text-align:none;
        margin-bottom:0px;
        }
        p {
        font-size:25px;
        text-align:none;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <details>
        <summary class="GFG">
            GeeksforGeeks
        </summary>
        <p>GeeksforGeeks is a Computer Science portal
            where you can learn good programming.
        </p>
    </details>
</body>

</html>
```

### Теги `<figure>` и `<figcaption>`

Теги `<figure>` и `<figcaption>` используются для добавления изображения на веб-страницу с небольшим описанием.

**Пример:** Ниже приведен пример использования тегов `<figure>` и `<figcaption>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Figcaption Tag</title>
    <style>
        h2 {
        Color:#006400;
        font-size:50px;
        Text-align:none;
        margin-bottom:0px;
        }
        p {
        font-size:25px;
        text-align:none;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <h2>GeeksforGeeks</h2>
    <figure>
        <img src="4.jpg" 
             alt="gfg" 
             style="width:20%">
        <figcaption>
          GeeksforGeeks Logo
          </figcaption>
    </figure>
</body>

</html>
```

### Тег `<header>`

Как следует из названия, тег `<header>` предназначен для заголовка секции или введения на странице. На одной странице может быть несколько заголовков.

**Пример:** Ниже приведен пример использования тега `<header>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Header Tag</title>
    <style>
        h1, h3 {
        Color:#006400;
        Text-align:left;
        margin-bottom:0px;
        }
        p {
        font-size:25px;
        text-align:left;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <article>
        <header>
            <h1>GeeksforGeeks</h1>
            <h3>GeeksforGeeks</h3>
            <p>A computer Science portal</p>
        </header>
    </article>
</body>

</html>
```

### Тег `<footer>`

Тег `<footer>` располагается внизу статьи или документа и может содержать контактную информацию, авторские права и т. д. На одной странице может быть несколько подвалов.

**Пример:** Ниже приведен пример использования тега `<footer>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>footer Tag</title>
    <style>
        p {
        font-size:25px;
        text-align:left;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <footer>
        <p>
            Posted by: GeeksforGeeks
        </p>

        <p>
            Contact: 
            <a href=
"https://www.geeksforgeeks.org">
                geeksforgeeks.org
            </a>.
        </p>
    </footer>
</body>

</html>
```

### Тег `<main>`

Тег `<main>` определяет основной контент документа. Содержимое внутри тега `<main>` должно быть уникальным.

**Пример:** Ниже приведен пример использования тега `<main>` в HTML.
```html
<!DOCTYPE html>
<html>

<head>
    <title>main Tag</title>
    <style>
        h1 {
        color:#006400;
        }
        p {
        font-size:25px;
        text-align:none;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <main>
        <h1>Important Residences</h1>
        <p>
            A few of them are 
            Rashtrapati Bhavan, 
            White House etc
        </p>

        <article>
            <h1>Rashtrapati Bhavan</h1>
            <p>
                It is the home of 
                the President of India.
            </p>
        </article>
        
        <article>
            <h1>The White House</h1>
            <p>
                It is the home of the 
                President of United
                States of America.
            </p>
        </article>
    </main>
</body>

</html>
```

### Тег `<section>`

Страница может быть разделена на секции, такие как Введение, Контактная информация, Подробности и т. д., и каждая из этих секций может быть оформлена в отдельном теге `<section>`.

**Пример:** Ниже приведен пример использования тега `<section>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>section Tag</title>
    <style>
        h1 {
        color:#006400;
        }
        p {
        font-size:25px;
        text-align:none;
        margin-top:0px;
        }
    </style>
</head>

<body>
    <section>
        <h1>Data Structure</h1>
        <p>
            Data Structure is a data
            organization and storage
            format that enables efficient
            access and modification.
        </p>
    </section>
    <section>
        <h1>Algorithm</h1>
        <p>
            A process or set of rules to
            be followed in calculations
            or other problem-solving
            operations, especially by
            a computer.
        </p>
    </section>
</body>

</html>
```

### Тег `<nav>`

Тег `<nav>` используется для определения набора навигационных ссылок в виде навигационной панели или меню.

**Пример:** Ниже приведен пример использования тега `<nav>`.
```html
<!DOCTYPE html>
<html>

<head>
    <title>nav Tag</title>
    <style>
        h1 {
        color:#006400;
        }
    </style>
</head>

<body>
    <h1>Navigation Bar</h1>
    <nav>
        <a href="/home/">
            Home
        </a> |
        <a href="/about-us/">
            About Us
        </a> |
        <a href="/data-structure/">
            Data Structure
        </a> |
        <a href="/operating-system/">
            Operating System
        </a>
    </nav>
</body>

</html>
```

### Тег `<mark>`

Тег `<mark>` используется для выделения текста.

**Пример:** Ниже приведен пример использования тега `<mark>` в HTML.
```html
<!DOCTYPE html>
<html>

<head>
    <title>mark Tag</title>
    <style>
        h1 {
        color:#006400;
        }
    </style>
</head>

<body>
    <h1>mark tag</h1>
    <p>
        GeeksforGeeks is a
        <mark>Computer Science</mark>
        portal
    </p>
</body>

</html>
```

### Несемантические элементы

Теги, такие как `<div>` и `<span>`, относятся к несемантическим категориям, так как их названия не указывают на тип содержимого внутри них.

#### Тег `<div>`

Тег `<div>` — это блочный элемент, представляющий собой раздел секции. Он используется как контейнер.

**Пример:** Ниже приведен пример использования несемантических элементов.
```html
<!DOCTYPE html>
<html>

<head>
    <title>div Tag</title>
    <style>
        .GFG {
        color:#006400;
        }
    </style>
</head>

<body>
    <h1>div Tag</h1>
    <div class="GFG">
        <h1>GeeksforGeeks</h1>
        <p>GeeksforGeeks is a Computer Science portal</p>
    </div>
</body>

</html>
```

### Тег `<span>`

Тег `<span>` — это строчный элемент, который не начинает новую строку и занимает только необходимую ширину.