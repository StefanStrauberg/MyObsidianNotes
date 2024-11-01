Тег HTML `<span>` — это встроенный контейнер, используемый для группировки и применения стилей или скриптов к определенным частям текста или элементов в документе.

Хотя сам по себе он не влияет на макет или внешний вид, он служит целью для CSS-стилей и взаимодействий с JavaScript, что делает его идеальным для настройки небольших частей контента без нарушения потока окружающих элементов.

**Синтаксис:**
```html
<span class="">Some Text</span>
```
>[!note]
>Тег HTML `<span>` поддерживаетс Global attribute и Event Attributes

### Примеры тега HTML `<span>`

Вот несколько примеров использования тега `<span>`:

**Пример 1: Упрощение кода и группировка стилей с помощью `<span>`**
В этом примере мы используем тег `<span>` для непосредственного применения CSS-стилей к определенному контенту, что позволяет сократить повторяющиеся HTML-атрибуты. Такой подход обеспечивает более чистый код и единый стиль для элементов.
```html
<!DOCTYPE html>
<html>
  <head>
    <title>GeeksforGeeks span tag</title>

    <!-- style for span tag  -->
    <style>
      span {
        color: green;
        text-decoration: underline;
        font-style: italic;
        font-weight: bold;
        font-size: 26px;
      }
    </style>
  </head>

  <body>
    <span> GeeksforGeeks </span><br />
    <span> GeeksforGeeks </span><br />
    <span> GeeksforGeeks </span><br />
  </body>
</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240529164125/spant.png)

**Пример 2: Встроенное поведение элементов `<span>`**
В этом примере тег `<span>` работает как встроенный элемент. Каждый `<span>` занимает только пространство, необходимое для его содержимого, что позволяет нескольким элементам `<span>` размещаться на одной строке, не влияя на общий макет.
```html
<!DOCTYPE html>
<html>

<head>
    <title>GeeksforGeeks span tag</title>
</head>

<body>

    <!-- span tags with inline style/css  -->
    <span style="background-color:powderblue;">
        GfG
    </span>
    <span style="background-color: lightgray;">
        -Contribute-
    </span>
    <span style="background-color: yellow;">
        Article
    </span>
    <span style="background-color: lightgreen;">
        GCET
    </span>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/20240529164353/span2.png)

**Зачем использовать тег `<span>`?**
Тег `<span>` — это универсальный встроенный элемент для группировки и стилизации текста или элементов в документе. Он позволяет применять CSS и JavaScript к определенным частям контента, что повышает гибкость и эффективность веб-дизайна и интерактивности. Поскольку он поддерживает глобальные и событийные атрибуты, тег `<span>` совместим со всеми основными браузерами, что делает его основным инструментом в современном веб-разработке.