# HTML-CSS
HTML &amp; CSS course at SoftUni - January 2024

[Click Here for more information about the course HTML & CSS](https://softuni.bg/trainings/4361/html-and-css-january-2024#lesson-64763)
<br/>
<br/>
![HTML   CSS](https://github.com/HristianBalevski/HTML-CSS/assets/114162692/9096de7f-6f71-4934-b8e7-1985fe91087f)

## 01.Introduction to HTML & CSS

**1. Какво е HTML?**

HTML (Hypertext Markup Language) е език за маркиране, който се използва за построяване на уеб страници. С други думи, HTML помага да структурираме информацията на страницата така, че браузърът да я разбира и показва правилно.

**2. HTML Синтаксис - Тагове и Атрибути**

HTML използва тагове, които се заключват в ъглови скоби < >. Таговете съдържат елементи на страницата и определят тяхната структура. Атрибутите предоставят допълнителна информация за елементите.

Пример:
```
<p class="example">Това е абзац с клас "example".</p>
```

**3. Общи HTML Тагове**

- `<h1>` to `<h6>`: Заглавия с различни размери.
- `<p>`: Параграф.
- `<a>`: Хипервръзка (линк).
- `<img>`: Изображение.
- `<ul>`, `<ol>`, `<li>`: Списъци.

**4. Общи HTML Атрибути**

- `class`: Добавя клас към елемента.
- `id`: Уникален идентификатор за елемента.
- `src`: За източник на изображение или хипервръзка.
- `href`: Указва адреса на хипервръзка.

**5. Какво е CSS?**

CSS (Cascading Style Sheets) се използва за стилизиране и форматиране на уеб страници. Той определя изгледа и оформлението на HTML елементите.

**6. CSS Синтаксис - Селектори и Правила**

CSS използва селектори за избор на HTML елементи и правила за дефиниране на техния вид. Правилата се състоят от свойства и стойности.

Пример:
```
/* Селектор */
p {
  /* Правило */
  color: blue;
}
```

**7. Добавяне на CSS към HTML документите**

Можем да добавим CSS в HTML документите чрез външни файлове, вътрешни стилове в тага `<style>` или дори чрез инлайн атрибути.

**8. Основни CSS Селектори**

- Елементен селектор: `p {}` - За всички параграфи.
- Класов селектор: `.example {}` - За елементи с клас "example".
- Идентификационен селектор: `#unique {}` - За елемент с идентификатор "unique".

---
## 02.HTML Structure

**1. Семантичен HTML**

Семантичният HTML включва използването на тагове, които не само определят структурата на уеб страници, но и предоставят смисъл и значение на съдържанието. Това помага не само на разработчиците, но и на търсачките и четящите уеб страницата да разберат по-добре нейната структура.

Пример:

```
<header>
  <h1>Заглавие на страницата</h1>
  <nav>
    <ul>
      <li><a href="#">Начало</a></li>
      <li><a href="#">За нас</a></li>
      <li><a href="#">Контакти</a></li>
    </ul>
  </nav>
</header>
```

**2. HTML Тагове**

a. `<div>` и `<span>`
 - `<div>` се използва за групиране на елементи, а `<span>` - за определяне на стилове или обграждане на текстове без да променя структурата.

Пример:

```
<div class="container">
  <p>Текст в контейнер</p>
  <span style="color: red;">Червен текст</span>
</div>
```

b. `<section>` и `<article>`
  - `<section>` се използва за групиране на тематично свързани елементи, а `<article>` - за конкретен самостоятелен материал.

Пример:

```
<section>
  <h2>Раздел</h2>
  <article>
    <h3>Статия 1</h3>
    <p>Съдържание на статията 1.</p>
  </article>
  <article>
    <h3>Статия 2</h3>
    <p>Съдържание на статията 2.</p>
  </article>
</section>
```

**3. Форми**

HTML формите се използват за събиране на информация от потребителите. Те включват различни елементи като текстови полета, бутони, радио бутони и др.

Пример:

```
<form action="/submit" method="post">
  <label for="username">Потребителско име:</label>
  <input type="text" id="username" name="username" required>

  <label for="password">Парола:</label>
  <input type="password" id="password" name="password" required>

  <button type="submit">Вход</button>
</form>
```

**4. Таблици**

Таговете за таблици (`<table>`, `<tr>`, `<th>`, `<td>`) се използват за представяне на информация в табличен формат.

Пример:

```
<table>
  <tr>
    <th>Име</th>
    <th>Години</th>
  </tr>
  <tr>
    <td>Иван</td>
    <td>25</td>
  </tr>
  <tr>
    <td>Мария</td>
    <td>22</td>
  </tr>
</table>
```

Тези основни концепции в HTML структурата помагат да се създадат уеб страници с чист и смислен код, които са лесни за разбиране и поддръжка.

---

## 03.CSS & Typography

**1. Типография**
Типографията в уеб дизайна се отнася до стиловете и атрибутите, които се прилагат към текста. Това включва избор на шрифтове, размери, интервали и цветове, които правят текста по-четим и естетичен.

Пример:

```
body {
  font-family: 'Arial', sans-serif;
  font-size: 16px;
  line-height: 1.5;
  color: #333;
}
```

**2. Принципи на Четливост**

  - **Размер на шрифта:** Използвайте подходящ размер за различните части от уеб страницата, като заглавия, подзаглавия и текст.
  - **Линейна височина:** Задайте подходяща височина на линията, за да подобрите четливостта и възприемчивостта на текста.
  - **Цветове:** Осигурете достатъчен контраст между текста и фона, за да улесните четенето.

**3. CSS Свойства**

a. `font-family`
Задава шрифт за елемент.

Пример:

```
h1 {
  font-family: 'Helvetica', sans-serif;
}
```

b. `font-size`
Задава размер на шрифта.

Пример:

```
p {
  font-size: 18px;
}
```
c. `line-height`

Задава височина на линията.

Пример:

```
body {
  line-height: 1.6;
}
```

d. `color`

Задава цвят на текста.

Пример:

```
h2 {
  color: #007bff;
}
```

**4. Font Awesome Икони**

Font Awesome предоставя набор от шрифтове и CSS класове, които представляват различни икони. Това позволява добавянето на икони без използване на изображения.

Пример:

```
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
</head>
<body>

  <i class="fas fa-heart"></i> <!-- Сърце икона -->

</body>
</html>
```

Тези инструменти и принципи са важни за създаване на четим и естетичен текст в уеб дизайна. От типографията до CSS свойствата и използването на икони, всичко това влияе на визуалния стил и усещането на уеб страницата.

---

## 04.CSS Box Model

**1. CSS Box Model**

CSS Box Model представлява начина, по който браузърът изчислява размерите на всеки HTML елемент. Той се състои от четири основни части: контент, padding, border и margin.

**2. Блокови и Вмъкваеми Елементи**

  - **Блокови елементи:** Заемат цялата налична ширина, започват на нов ред и имат възможност да имат вложени елементи.

    Пример:
    
    ```
    div {
      display: block;
    }
    ```
  - **Вмъкваеми (Inline) елементи:** Заемат само толкова ширина, колкото е необходима, не започват на нов ред и не допускат вътрешни вложени елементи.

    Пример:

    ```
    span {
      display: inline;
    }
    ```

**3. Ширина и Височина**

  - Ширина и Височина: Задават се със свойствата `width` и `height`.
    
    Пример:

    ```
    .box {
      width: 200px;
      height: 150px;
      }
    ```
**4. Padding, Margin и Border**

  - **Padding (Отстъп):** Отстъпът между границата на елемента и неговото съдържание.

    Пример:

    ```
    .box {
      padding: 20px;
      }
    ```
 - **Margin (Външен Отстъп):** Отстъпът от границата на елемента до околните елементи.

   Пример:

   ```
   .box {
      margin: 10px;
    }
   ```
- **Border (Граница):** Границата около елемента.

  Пример:

  ```
  .box {
      border: 1px solid #ccc;
   }
  ```

**5. Box Sizing**

`box-sizing` свойството определя как браузърът изчислява общия размер на елемента, включително padding и border.

- **Content-Box (Стандарт):** Ширината и височината включват само съдържанието, без padding и border.

  ```
  .box {
    box-sizing: content-box;
   }  
  ```

- **Border-Box:** Ширината и височината включват съдържание, padding и border.

  ```
  .box {
    box-sizing: border-box;
   }
  ```

  Това са основните аспекти на CSS Box Model. Те са важни при стилизирането и позиционирането на елементите в уеб дизайна.

  ---
  



