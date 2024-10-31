### Атрибуты HTML

Атрибуты HTML предоставляют дополнительную информацию об элементах в HTML-документе. Каждый HTML-элемент может иметь атрибуты, которые определяются в открывающем теге. Атрибуты указываются в формате пары имя/значение, где имя атрибута определяет свойство, а его значение предоставляет конкретные детали, например, `name="value"`. Эти атрибуты влияют на отображение контента и взаимодействие на веб-страницах.

### Компоненты атрибута HTML

Атрибут HTML состоит из двух основных компонентов:

| Attribute Name  | Description                                                                                                                        |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| id              | Уникальный идентификатор для элемента HTML, используемый для стилизации или взаимодействия с JavaScript.                           |
| class           | Определяет одно или несколько имен классов для элемента, используемых для стилизации и применения CSS-правил.                      |
| src             | Указывает URL-адрес источника для внешних ресурсов, таких как изображения, аудио или видео.                                        |
| href            | Указывает URL-адрес связанного ресурса, обычно используется в элементах `<a>` для гиперссылок.                                     |
| alt             | Предоставляет альтернативный текст для изображений, который отображается, если изображение не может быть загружено или недоступно. |
| any_custom_attr | Описывает любое пользовательское имя атрибута и его назначение в HTML-документе.                                                   |

Синтаксис:
```html
<element attribute_name="attribute_value">
```

### Атрибуты мета-тегов

Мета-теги предоставляют важную информацию о HTML-документах. Это самозакрывающиеся теги, которые значительно влияют на функциональность браузера, SEO, определение кодировки символов и управление отображением. Вот некоторые часто используемые атрибуты мета-тегов:

| Attribute  | Description                                                                                       |
| ---------- | ------------------------------------------------------------------------------------------------- |
| charset    | Определяет кодировку символов для HTML-документа.                                                 |
| name       | Указывает имя атрибута метаданных.                                                                |
| content    | Устанавливает HTTP-заголовок для содержимого, обычно используется для обратной совместимости.     |
| http-equiv | Указывает формат, используемый для интерпретации значения                                         |
| scheme     | Указывает формат, используемый для интерпретации значения содержимого, часто для форматов данных. |

### Глобальные атрибуты HTML

Глобальные атрибуты применяются ко всем типам HTML-тегов. Вот некоторые часто используемые глобальные атрибуты:

| Attribute       | Description                                                                                                                                                |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| class           | Группирует элементы и позволяет применять стили.                                                                                                           |
| style           | Встраивает CSS-стили.                                                                                                                                      |
| src             | Указывает источник различных ресурсов, таких как URL-адреса изображений для элемента `<img>`, видео для элемента `<video>` и аудио для элемента `<audio>`. |
| contenteditable | Определяет, можно ли редактировать содержимое элемента.                                                                                                    |
| role            | Указывает роль элемента для доступности.                                                                                                                   |
| tabindex        | Определяет порядок фокуса при навигации с помощью клавиатуры.                                                                                              |
| id              | Присваивает уникальный идентификатор элементу, позволяя нацеливаться на него с помощью CSS или JavaScript.                                                 |
| href            | Определяет адрес гиперссылки в элементе `<a>`, обеспечивая навигацию.                                                                                      |
| alt             | Предоставляет альтернативный текст для изображений, что важно для доступности и SEO.                                                                       |
| title           | Создает всплывающую подсказку, которая появляется при наведении курсора на элемент.                                                                        |
| lang            | Указывает язык содержимого элемента, что помогает с переводом и доступностью.                                                                              |

### Атрибут src в HTML

Атрибут `src` в HTML указывает URL-адрес ресурса (например, изображения, аудио или видео), который будет встроен или включен в веб-страницу.

**Пример:** Этот пример демонстрирует использование атрибута `src` для указания адреса файла.
```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML img src Attribute</title>
</head>

<body>
    <img src=
"https://media.geeksforgeeks.org/wp-content/cdn-uploads/Geek_logi_-low_res.png">
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510112340/HTML-Attributes.png)
### Атрибут alt в HTML

Атрибут `alt` в HTML предоставляет альтернативный текст для изображения, если оно не может быть отображено. Это улучшает доступность и предоставляет контекст для экранных считывателей.

**Пример:** Этот пример демонстрирует использование атрибута `alt` для указания имени файла, когда изображение не загружается должным образом.
```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML img alt Attribute</title>
</head>

<body>

    <!--If the image is not found or the img field 
     is left blank the alt value gets displayed-->

    <img src=
"https://media.geeksforgeeks.org/wp-content/cdn-uploads/Geek_logi_-low_res.png" 
         alt="The Logo"><br>
    <img src="" 
         alt="Since the src value is blank,the alt value is displayed">
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510112500/HTML-Attributes-1.jpg)
### Атрибуты width и height в HTML

Атрибуты `width` и `height` используются для настройки ширины и высоты изображения (в пикселях).

**Пример:** Этот пример демонстрирует использование атрибутов `width` и `height` для указания различных размеров изображений.
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Width and Height</title>
</head>

<body>
    <img src=
"https://media.geeksforgeeks.org/wp-content/cdn-uploads/Geek_logi_-low_res.png"
         width="300px"
         height="100px">
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510112611/HTML-Attributes-2.jpg)
### Атрибут id в HTML

Атрибут `id` в HTML присваивает уникальный идентификатор элементу, что позволяет нацеливаться на него с помощью CSS и JavaScript для стилизации и манипуляции.

**Пример:** Этот пример демонстрирует использование атрибута `id` для указания уникального значения для конкретного элемента.
```html
<!DOCTYPE html>
<html>

<head>
    <style>
        #geeks {
            color: green;
        }
    </style>
</head>

<body>
    <h1 id="geeks">Welcome to GeeksforGeeks</h1>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510112944/HTML-Attributes-Example.png)
### Атрибут title в HTML

Атрибут `title` используется для пояснения элемента при наведении мыши на него. Поведение может различаться в зависимости от элементов, но обычно значение отображается при загрузке или при наведении курсора.

**Пример:** Этот пример демонстрирует использование атрибута `title` для указания метаданных элемента при наведении мыши.
```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML title Attribute</title>
</head>

<body>
    <h3 title="Hello GeeksforGeeks">
        Hover to see the effect
    </h3>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Untitled-5.jpg)
### Атрибут href в HTML

Атрибут `href` в HTML, используемый с тегом `<a>`, указывает адрес назначения ссылки. При нажатии на связанный текст происходит переход по этому адресу. Добавление `target="_blank"` открывает ссылку в новой вкладке.

**Пример:** Этот пример демонстрирует использование атрибута `href` для указания адреса файла ссылки.
```html
<!DOCTYPE html>
<html>

<head>
    <title>link Attribute</title>
</head>

<body>
    <a href="https://www.geeksforgeeks.org/">
        Click to open in the same tab
    </a><br>
    <a href="https://www.geeksforgeeks.org/" 
       target="_blank">
        Click to open in a different tab
    </a>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/al-1.jpg)
### Атрибут style в HTML

Атрибут `style` используется для применения различных эффектов CSS к HTML-элементам, таких как изменение размера шрифта, шрифта, цвета и т. д.

**Пример:** Этот пример демонстрирует использование атрибута `style` для указания свойств стиля для HTML-элемента.
```html
<!DOCTYPE html>
<html>

<head>
    <title>style Attribute</title>
</head>

<body>
    <h2 style="font-family:Chaparral Pro Light;">
          Hello GeeksforGeeks.
      </h2>
    <h3 style="font-size:20px;">
          Hello GeeksforGeeks.
      </h3>
    <h2 style="color:#8CCEF9;">
          Hello GeeksforGeeks.
      </h2>
    <h2 style="text-align:center;">
          Hello GeeksforGeeks.
      </h2>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510113457/HTML-style-Attribute.jpg)
### Атрибут lang в HTML

Атрибут `lang` используется для указания языка документа. Объявление языка важно для приложений доступности и поисковых систем, так как помогает правильно интерпретировать содержимое.

**Пример:** Этот пример демонстрирует использование атрибута `lang` для указания языка HTML-страницы.
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content=
              "width=device-width, initial-scale=1.0">
    <title>lang attribute</title>
    <style>
        body {
            text-align: center;
        }

        h1 {
            color: green;
        }

        .lang-info {
            font-style: italic;
        }
    </style>
</head>

<body>
    <h1>GeeksforGeeks</h1>
    <h2>lang attribute</h2>

    <p lang="en">
        A computer science portal for geeks
    </p>

    <p lang="fr" class="lang-info">
        A computer science portal for geeks
    </p>

    <p lang="es" class="lang-info">
        A computer science portal for geeks
    </p>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240510113317/HTML-lang-attribute.png)