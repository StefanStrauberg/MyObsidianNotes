### Тег `<caption>` в HTML

Тег `<caption>` используется для указания заголовка (подписи) таблицы. Важно помнить, что для каждой таблицы можно указать только одну подпись. По умолчанию она выравнивается по центру и располагается сразу после тега `<table>`, перед любыми элементами `<tr>` или `<th>`.

### Основные моменты
- **Структура**: Подпись добавляется непосредственно после открытия тега `<table>`.
- **Выравнивание**: Подпись по умолчанию выравнивается по центру.
- **Количество**: Каждая таблица может содержать только одну подпись.

**Синтаксис:**
```html
<caption align = "value" ></caption>
```

### Атрибуты:

| Attribute Value | Description                                                                                                                                                                                                                                                                                                                                            |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| align           | Атрибут `align` использовался для указания выравнивания текстового содержимого в элементах HTML, таких как заголовки ячеек (`<th>`) и стандартные ячейки (`<td>`). Однако этот атрибут был **устаревшим** (deprecated) в HTML5, и его использование не рекомендуется. Вместо этого рекомендуется использовать CSS для управления выравниванием текста. |

***Пример 1:*** Добавление подписи к таблице с центровкой по умолчанию
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>HTML5 caption Tag</title>
</head>

<body>
    <h1>GeeksForGeeks</h1>
    <h2>HTML &lt;Caption Tag&gt;</h2>

    <table>
        <!-- Adding caption to the table -->
        <caption>Students</caption>
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
![](https://media.geeksforgeeks.org/wp-content/uploads/20210208120049/caption.png)

***Пример 2:*** Добавление подписи к таблице с выравниванием влево
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>HTML5 caption Tag</title>
</head>

<body>
    <h1>GeeksForGeeks</h1>
    <h2>HTML &lt;Caption Tag&gt;</h2>

    <table>
        <!-- Adding a caption to the table 
        and aligning it to the left-->
        <caption style="text-align: left">
            Students
        </caption>
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
![](https://media.geeksforgeeks.org/wp-content/uploads/20210208120113/caption2.png)
