HTML-таблицы — это мощный инструмент для представления данных на вашем сайте. Однако их использование выходит за рамки простых строк и столбцов. 

### Что такое HTML-таблицы?

HTML-таблица — это организация данных в строках и столбцах в табличном формате. Таблицы полезны для представления текстовой информации и числовых данных, а также для быстрого нахождения связей между различными типами данных. Их также используют для создания баз данных.
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<body>
    <table>
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20210910153459/1230.png)
### Теги, используемые в HTML-таблицах

| HTML Tags                       | Descriptions                                                                                     |
| ------------------------------- | ------------------------------------------------------------------------------------------------ |
| `<table>`                       | Определяет структуру для организации данных в строках и столбцах на веб-странице.                |
| [[HTML tr Tag\|<tr>]]           | Представляет строку таблицы, содержащую ячейки.                                                  |
| [[HTML th Tag\|<th>]]           | Обозначает заголовочную ячейку, обычно содержащую названия или заголовки.                        |
| `<td>`                          | Представляет стандартную ячейку данных, содержащую информацию или данные.                        |
| [[HTML caption Tag\|<caption>]] | Предоставляет заголовок или описание для всей таблицы.                                           |
| `<thead>`                       | Определяет заголовочную секцию таблицы, часто содержащую метки столбцов.                         |
| `<tbody>`                       | Представляет основную область содержания таблицы, отделяя её от заголовка и нижнего колонтитула. |
| `<tfoot>`                       | Определяет нижний колонтитул таблицы, обычно содержащий сводки или итоги.                        |
| `<col>`                         | Определяет атрибуты для столбцов таблицы, применимые к нескольким столбцам одновременно.         |
| `<coldgroup>`                   | Группирует набор столбцов в таблице, к которым можно применять форматирование или свойства.      |

### Определение таблиц в HTML

HTML-таблица определяется с помощью тега **`<table>`**. Каждая строка таблицы обозначается тегом [[HTML tr Tag|<tr>]], а заголовок таблицы — тегом **`<th>`**. Заголовки таблицы по умолчанию отображаются жирным шрифтом и по центру. Ячейка данных таблицы определяется тегом **`<td>`**.

### Ячейки таблицы

Ячейки таблицы являются основными элементами для её определения. Они обозначаются тегами **`<td>`** (начальный) и **`</td>`** (конечный).  
**Синтаксис:**
```html
<td>Содержимое...</td>
```

### Строки таблицы

Строки формируются с помощью комбинации ячеек таблицы, обозначаются тегами **[[HTML tr Tag|<tr>]]** (начальный) и **[[HTML tr Tag|</tr>]]** (конечный).  
**Синтаксис:**
```html
<tr>Содержимое...</tr>
```

### Заголовки таблицы

Заголовки обычно используются для предоставления заголовка. Они могут добавляться в таблицу с помощью тегов **`<th>`** (начальный) и **`</th>`** (конечный).  
**Синтаксис:**
```html
<th>Содержимое...</th>
```

**Пример**: создания простой таблицы
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<body>
    <table>
        <tr>
            <th>Book Name</th>
            <th>Author Name</th>
            <th>Genre</th>
        </tr>
        <tr>
            <td>The Book Thief</td>
            <td>Markus Zusak</td>
            <td>Historical Fiction</td>
        </tr>
        <tr>
            <td>The Cruel Prince</td>
            <td>Holly Black</td>
            <td>Fantasy</td>
        </tr>
        <tr>
            <td>The Silent Patient</td>
            <td> Alex Michaelides</td>
            <td>Psychological Fiction</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20210910153420/1157.png)
### Добавление рамки к HTML-таблице

Рамка устанавливается с помощью CSS-свойства `border`. Если вы не зададите рамку для таблицы, она будет отображаться без рамок.
**Синтаксис:**
```css
table, th, td {  
      border: 1px solid black;  
}
```

**Пример**: Добавление рамки к HTML-таблице
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
        }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-15-at-10.45.20-AM.png)
### Добавление схлопнутых границ в HTML-таблице

Чтобы рамки таблицы схлопнулись в одну, используйте CSS-свойство `border-collapse`
**Синтаксис:**
```css
table, th, td {  
       border: 1px solid black;  
       border-collapse: collapse;  
   }
```

**Пример**: Добавление схлопнутых схлопнутых к HTML-таблице
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
    table,
    th,
    td {
        border: 1px solid black;
        border-collapse: collapse;
    }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-15-at-10.49.53-AM.png)
### Добавление отступов в ячейках HTML-таблицы

Отступы ячеек (cell padding) определяют пространство между содержимым ячейки и её границами. Если отступы не заданы, ячейки таблицы будут отображаться без отступов.
**Синтаксис:**
```css
th, td {  
        padding: 20px;  
}
```

**Пример**: Добавление отступов в ячейках HTML-таблицы
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
    table,
    th,
    td {
        border: 1px solid black;
        border-collapse: collapse;
    }
    
    th,
    td {
        padding: 20px;
    }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-15-at-7.26.30-PM.png)
### Добавление выравнивания заголовков таблицы влево

По умолчанию заголовки таблицы отображаются жирным шрифтом и по центру. Чтобы выровнять заголовки таблицы по левому краю, необходимо использовать свойство CSS `text-align`.

**Синтаксис:**
```css
th {  
      text-align: left;  
}
```

**Пример**: Добавление свойства выравнивания где текст выравнивается влево
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-collapse: collapse;
        }

        th,
        td {
            padding: 20px;
        }

        th {
            text-align: left;
        }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-3.40.39-PM.png)
### Добавление расстояния между границами в HTML-таблице

Расстояние между границами (border spacing) определяет пространство между ячейками таблицы. Чтобы установить расстояние между границами для таблицы, необходимо использовать CSS-свойство `border-spacing`.

**Синтаксис:**
```css
table {  
      border-spacing: 5px;  
}
```

**Пример**: Добавление свойства `border-spacing` для создания пространства между ячейками таблицы
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
        }

        table {
            border-spacing: 5px;
        }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-3.45.40-PM.png)
### Добавление ячеек, охватывающих несколько столбцов в HTML-таблицах

Чтобы сделать ячейку, которая охватывает более одного столбца, необходимо использовать атрибут `colspan`. Этот атрибут позволяет указать, сколько столбцов должна занимать ячейка.

**Пример**: Использование атрибута `colspan` 
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-collapse: collapse;
        }

        th,
        td {
            padding: 5px;
            text-align: left;
        }
    </style>
</head>

<body>
    <h2>Cell that spans two columns:</h2>
    <table style="width:100%">
        <tr>
            <th>Name</th>
            <th colspan="2">Telephone</th>
        </tr>
        <tr>
            <td>Vikas Rawat</td>
            <td>9125577854</td>
            <td>8565557785</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-3.49.33-PM.png)
### Добавление ячеек, охватывающих несколько строк в HTML-таблицах

Чтобы создать ячейку, которая охватывает более одной строки, необходимо использовать атрибут `rowspan`. Этот атрибут позволяет указать, сколько строк должна занимать ячейка.

**Пример**: Использование атрибута `rowspan`
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-collapse: collapse;
        }

        th,
        td {
            padding: 5px;
            text-align: left;
        }
    </style>
</head>

<body>
    <h2>Cell that spans two rows:</h2>
    <table style="width:100%">
        <tr>
            <th>Name:</th>
            <td>Vikas Rawat</td>
        </tr>
        <tr>
            <th rowspan="2">Telephone:</th>
            <td>9125577854</td>
        </tr>
        <tr>
            <td>8565557785</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-3.53.18-PM.png)
### Добавление заголовка к HTML-таблице

Чтобы добавить заголовок к таблице, необходимо использовать тег `<caption>`. Этот тег позволяет задать описание или название таблицы, которое будет отображаться сверху.

**Пример**: Добавление заголовка к HTML-таблице
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-collapse: collapse;
        }

        th,
        td {
            padding: 20px;
        }

        th {
            text-align: left;
        }
    </style>
</head>

<body>
    <table style="width:100%">
        <caption>DETAILS</caption>
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-4.12.02-PM.png)
### Добавление фона к таблице в HTML

Цвет фона можно добавить в таблицу HTML с помощью свойства CSS `background-color`. Это позволяет улучшить визуальное восприятие таблицы и выделить её содержание.

**Синтаксис:**
```css
table#t01 {  
            width: 100%;  
            background-color: #f2f2d1;  
 }
```

**Пример**: Добавление фона к HTML-таблице
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<head>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-collapse: collapse;
        }

        th,
        td {
            padding: 5px;
            text-align: left;
        }

        table#t01 {
            width: 100%;
            background-color: #f2f2d1;
        }
    </style>
</head>

<body>
    <table style="width:100%">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
    <br />
    <br />
    <table id="t01">
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Age</th>
        </tr>
        <tr>
            <td>Priya</td>
            <td>Sharma</td>
            <td>24</td>
        </tr>
        <tr>
            <td>Arun</td>
            <td>Singh</td>
            <td>32</td>
        </tr>
        <tr>
            <td>Sam</td>
            <td>Watson</td>
            <td>41</td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-4.16.23-PM.png)
### Создание вложенных таблиц

Вложенные таблицы означают создание таблицы внутри другой таблицы. Это позволяет создавать более сложные макеты таблиц, которые могут быть визуально интересными, но также могут увеличить риск ошибок при разметке.

**Пример**: Создание вложенных таблиц
```html
<!-- index.html -->
<!DOCTYPE html>
<html>

<body>
    <table border=5 bordercolor=black>
        <tr>
            <td> First Column of Outer Table </td>
            <td>
                <table border=5 bordercolor=grey>
                    <tr>
                        <td> First row of Inner Table </td>
                    </tr>
                    <tr>
                        <td> Second row of Inner Table </td>
                    </tr>
                </table>
            </td>
        </tr>
    </table>
</body>

</html>
```
![](https://media.geeksforgeeks.org/wp-content/uploads/Screen-Shot-2017-11-16-at-4.29.26-PM.png)
