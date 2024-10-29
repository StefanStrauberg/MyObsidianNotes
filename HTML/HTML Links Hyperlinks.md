### HTML ссылки (гиперссылки)

HTML ссылки, или гиперссылки, соединяют веб-страницы и создаются с помощью тега `<a>` с атрибутом `href`. Они позволяют пользователям перемещаться между страницами или ресурсами. Ссылки могут быть текстовыми, графическими или представлять собой другие элементы, улучшая навигацию и интерактивность веба. Пользователи могут кликать на ссылки для перехода на разные страницы или ресурсы.

_Примечание: Гиперссылка может быть представлена изображением или любым другим элементом HTML, а не только текстом._

### По умолчанию ссылки отображаются следующим образом:

- **Несуществующая ссылка**: подчеркнута и синяя.
- **Посещенная ссылка**: подчеркнута и пурпурная.
- **Активная ссылка**: подчеркнута и красная.

**Синтаксис:**
```html
<a href="url">link text</a>
```

### Target атрибуты

| Attribute   | Description                                                                                   |
| ----------- | --------------------------------------------------------------------------------------------- |
| `_blank`    | Открывает связанный документ в новом окне или вкладке.                                        |
| `_self`     | Открывает связанный документ в том же окне или фрейме, что и ссылка. (Поведение по умолчанию) |
| `_parent`   | Открывает связанный документ в родительском фрейме.                                           |
| `_top`      | Открывает связанный документ в полном теле окна.                                              |
| `framename` | Открывает связанный документ в указанном фрейме, имя которого задаётся в атрибуте.            |
|             |                                                                                               |

### Примеры HTML ссылок

**Пример 1: Базовая гиперссылка**

В этом примере содержится параграф, который призывает пользователей кликнуть по ссылке "GeeksforGeeks", которая перенаправляет на сайт “https://www.geeksforgeeks.org”:
```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Links</title>
</head>

<body>
    <p>Click on the following link</p>
    <a href="https://www.geeksforgeeks.org">
        GeeksforGeeks
    </a>
</body>

</html>
```

**Пример 2: Использование атрибутов target**

В этом примере демонстрируется использование атрибутов target в ссылках. Каждая ссылка открывается в различном контексте:
```html
<!DOCTYPE html>
<html>

<head>
    <title>Target Attribute Example</title>
</head>

<body>
    <h3>
        Various options available in the
        Target Attribute
    </h3>

    <p>
        If you set the target attribute to
        "_blank", the link will open in a new
        browser window or tab.
    </p>
    <a href="https://www.geeksforgeeks.org" 
       target="_blank">
        GeeksforGeeks
    </a>

    <p>
        If you set the target attribute to
        "_self", the link will open in the
        same window or tab.
    </p>
    <a href="https://www.geeksforgeeks.org" 
       target="_self">
        GeeksforGeeks
    </a>

    <p>
        If you set the target attribute to
        "_top", the link will open in the full
        body of the window.
    </p>
    <a href="https://www.geeksforgeeks.org" 
       target="_top">
        GeeksforGeeks
    </a>

    <p>
        If you set the target attribute to
        "_parent", the link will open in the
        parent frame.
    </p>
    <a href="https://www.geeksforgeeks.org" 
       target="_parent">
        GeeksforGeeks
    </a>
</body>

</html>
```
