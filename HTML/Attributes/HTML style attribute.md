В этой статье мы рассмотрим атрибут стиля HTML и поймем его реализацию через примеры. Стили в HTML — это правила, которые описывают, как документ будет представлен в браузере. Информация о стилях может быть либо прикреплена как отдельный документ, либо встроена в HTML-документ. Существуют три способа реализации стилей в HTML:

**Содержание:**
- Inline Style (Встроенный стиль)
- Embedded Style (Встроенный стиль)
- External Style Sheet (Внешняя таблица стилей)

**Поддерживаемые теги:**
Атрибут стиля поддерживается всеми элементами HTML.

### Inline Style:
При использовании встроенных стилей правила CSS записываются непосредственно в стартовом теге с помощью атрибута style. Атрибут style включает в себя набор свойств CSS и соответствующих значений. Каждая пара "свойство: значение" отделяется точкой с запятой (;). Этот атрибут переопределяет свойства стиля глобально для любых соответствующих стилей.

**Пример:** Этот пример описывает Inline Style, указывая атрибут style для добавления различных свойств стиля.
```html
<!DOCTYPE html>
<html>

<head>
    <title>Inline Styling</title>
</head>

<body>
    <h1 style="color:Blue;font-size:25px;">
        Example of Inline Style
    </h1>
    <p style="color:red;">First paragraph</p>

    <p style="color:green;font-size:40px;">
        Second paragraph
    </p>
    <hr style="border-color:orange;">
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-12-16-at-8.27.52-PM.png)

### Embedded Style:

Встроенные или внутренние таблицы стилей влияют только на документ, в который они встроены. Встроенные таблицы стилей определяются в разделе `<head>` HTML-документа с помощью тега `<style>`.

**Пример:** Этот пример демонстрирует свойства встроенного стиля.
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <style type="text/css">
        body {
            background-color: powderblue;
        }

        h1 {
            color: black;
            font-family: arial;
        }

        p {
            color: yellow;
            font-family: verdana;
        }
    </style>
    <title>Embedded Styling</title>
</head>

<body>
    <h1>Example of Embedded Style</h1>
    <p>First paragraph.</p>

</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-12-16-at-8.36.33-PM.png)

### External Style Sheet:

Метод внешних таблиц стилей полезен, когда CSS необходимо применить к нескольким веб-страницам. Внешная таблица стилей содержит все правила стилей в отдельном документе, который можно подключить из HTML-файла на вашем сайте. Существуют два способа подключения внешних таблиц стилей:

1. **Подключение внешних таблиц стилей**
2. **Импорт внешних таблиц стилей**

#### Подключение внешних таблиц стилей:

В этом методе внешняя таблица стилей связывается с HTML-документом с помощью тега `<link>`.

**Пример:** Этот пример демонстрирует использование внешней таблицы стилей для добавления различных свойств стиля.
```html
<!DOCTYPE html>
<html>

<head>
    <link rel="stylesheet" type="text/css" 
          href="/html/css/externalstyle.css">
    <title>External Styling</title>
</head>

<body>
    <h3>Example of Linking External Style Sheet</h3>
    <p>First paragraph.</p>

</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-12-16-at-8.43.06-PM.png)

### Импорт внешних таблиц стилей:

Внешние таблицы стилей можно загрузить в HTML-документ с помощью инструкции `@import`. Эта инструкция сообщает браузеру загрузить CSS-файл. Также можно включить другие правила CSS с помощью элемента `<style>`.

**Пример:** Этот пример демонстрирует использование импорта внешней таблицы стилей для добавления свойств стиля из внешнего стиля.
```html
<!DOCTYPE html>
<html>

<head>
    <style type="text/css">
        @import url("/html/css/importstyle.css");

        p {
            color: powderblue;
            font-size: 30px;
        }
    </style>
    <title>Importing external Styling</title>
</head>

<body>
    <h3>Example of external style sheet using import</h3>
    <p>First paragraph</p>

</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-12-16-at-9.38.41-PM.png)
