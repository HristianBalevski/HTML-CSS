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
**05. Какво представляват em и rem**
В CSS, **em** и **rem** са мерни единици, които се използват за измерване на разстояния, например размери на шрифт, отстъпи и др.
1. **em (от "emphasis"):**
   - **Как работи?** Размерът на **em** се изчислява въз основа на текущия размер на шрифта на елемента, на който се прилага.
   - **Пример:** Ако размерът на шрифта на родителския елемент е 16 пиксела, и ако имаме текст с размер на шрифта 2em, този текст ще бъде с размер 32 пиксела (16 * 2).
2. **rem (от "root emphasis"):**
   - **Как работи?** Размерът на rem се изчислява въз основа на размера на шрифта на кореновия (root) елемент, т.е., обикновено това е размерът на шрифта, зададен на HTML елемента.
   - **Пример:** Ако размерът на шрифта на HTML елемента е 16 пиксела, и ако имаме текст с размер на шрифта 2rem, този текст ще бъде с размер 32 пиксела (16 * 2).

Примерен HTML и CSS код:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>em vs rem</title>
  <style>
    body {
      font-size: 16px; /* Задава размер на шрифта на HTML елемента */
    }

    .parent {
      font-size: 1.5em; /* Задава размер на шрифта на елемента с клас "parent" */
    }

    .child-em {
      font-size: 2em; /* Размер на шрифта е 2 пъти текущият размер (1.5em * 2) */
    }

    .child-rem {
      font-size: 2rem; /* Размер на шрифта е 2 пъти размера на шрифта на HTML елемента (16px * 2) */
    }
  </style>
</head>
<body>
  <div class="parent">
    <p class="child-em">Text with em</p>
    <p class="child-rem">Text with rem</p>
  </div>
</body>
</html>
```
В този пример, текстът с **class="child-em"** ще бъде с размер 2 пъти по-голям от размера на шрифта на родителския елемент (1.5em * 2), докато текстът с **class="child-rem"** ще бъде с размер 2 пъти по-голям от размера на шрифта на HTML елемента (16px * 2).

Тези инструменти и принципи са важни за създаване на четим и естетичен текст в уеб дизайна. От типографията до CSS свойствата и използването на икони, всичко това влияе на визуалния стил и усещането на уеб страницата.

---

## 04.CSS Box Model

**1. CSS Box Model**

CSS Box Model представлява начина, по който браузърът изчислява размерите на всеки HTML елемент. Той се състои от четири основни части: контент, padding, border и margin.

**2. Блокови и Вмъкваеми Елементи**

  - CSS свойството **display** се използва за контролиране на начина, по който елементите се показват в документа. То позволява на дизайнера да управлява модела на разположение на елементите, включително дали елементът е блоков, линеен или друг тип.

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

  **06. Position**
  
  - Свойството **position** определя типа позициониране, използвано за елемента (**static**, **relative**, **fixed**, **absolute** or **sticky**).
  - След това елементите се позиционират чрез свойствата top, bottom, left и right.
  - Все пак тези свойства няма да функционират, освен ако първо не бъде зададено свойство за позициониране. Те също така работят по различен начин в зависимост от      стойността на свойството за позициониране.
 
**CSS Position**

- **position: static**;
  - Стандартното състояние на всеки елемент просто означава "постави елемента в неговата нормална позиция в потока на документа".
    ```
    .box {
        position: static;
        }
    ```

- **position: relative;**
  - Много сходно със статичното позициониране, с изключение, че след като позиционираният елемент заеме своето място в нормалния поток на оформлението на документа, можете да промените неговата окончателна позиция, включително правенето му да се застъпва с други елементи на страницата.

    ```
    .box {
    position: relative;
    }
    ```

- **position: absolute;**
  - По този начин трябва да позиционираме елемента въз основа на двумерна координатна система.
  - Можем да използваме **left**, **top**, **bottom**, **right**, за да поставим елемента точно там, където искаме.
     ```
    .box {
    position: absolute;
    }
     ```

- **position: fixed;**
  - Елементът се премахва от нормалния поток на документа и за него не се създава пространство в страницата.
  - Елементът се позиционира относително на своя начален контейнерен блок, който в случая на визуални медии е гледката (viewport).
  - Неговата окончателна позиция се определя от стойностите на top, right, bottom и left.
  - Тази стойност винаги създава нов контекст за наслояване (stacking context).
  - В печатни документи елементът се поставя на същата позиция на всяка страница.
 
      ```
      .box {
      position: fixed;
      }
      ```
- **position: sticky;**
  - Елементът се позиционира в съответствие с нормалния поток на документа, след което се отмества относително до неговия най-близък предшественик и контейнерен блок, включително елементите, свързани с таблица, в зависимост от стойностите на top, right, bottom и left.
  - Отместването не влияе на позицията на други елементи.
    ```
    .box {
    position: sticky;
    }
    ```

- **position: sticky;**
  - Тази стойност винаги създава нов контекст за наслояване (stacking context).
    ```
    .box {
    position: sticky;
    }
    ```

- z-index
  - Свойството z-index в CSS задава z-реда на позициониран елемент и неговите наследници или елементи на flex контейнер.
  - Елементите, които се застъпват и имат по-голям z-index, покриват тези с по-малък.
    ```
    .box {
    z-index: [number];
    }
    ```

  Това са основните аспекти на CSS Box Model. Те са важни при стилизирането и позиционирането на елементите в уеб дизайна.

---

## 05.Flexbox

- **Flexbox** е модул от CSS, който позволява да се подреждат елементите в контейнер по гъвкав начин. Той се използва за подравняване на елементите в една или повече редове или колони, както и за задаване на техния размер и разстояние един от друг.
- **Properties for the Parent** са свойствата, които се прилагат към контейнера, който съдържа елементите, подредени с flexbox. Тези свойства определят начина, по който елементите ще бъдат подредени.
- **Properties for the Children** са свойствата, които се прилагат към отделните елементи, подредени с flexbox. Тези свойства определят как всеки елемент ще се държи в контейнера.
 
**Ето някои от най-важните аспекти на flexbox:**

- **Flex-direction** определя посоката, в която ще бъдат подредени елементите. Може да бъде **row, column, row-reverse** или **column-reverse**.
---
- **Flex-wrap** определя дали елементите ще се обръщат, ако не се поберат в контейнера. Може да бъде nowrap, **wrap** или **wrap-reverse**.
---
- **Justify-content** определя как елементите ще бъдат подравнени по хоризонтала. Може да бъде **flex-start, flex-end, center, space-between, space-around** или **space-evenly**.
---
- **Align-items** определя как елементите ще бъдат подравнени по вертикала. Може да бъде **flex-start, flex-end, center, stretch** или **baseline**.

**Ето примерен код за използване на flexbox:**

HTML
```
<div class="container">
  <div class="item">Елемент 1</div>
  <div class="item">Елемент 2</div>
  <div class="item">Елемент 3</div>
</div>
```
CSS
```
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.item {
  width: 100px;
  height: 100px;
  background-color: red;
}
```
Този код ще подреди елементите в един ред, като остави равно разстояние между тях.

**Ето още един примерен код:**

HTML
```
<div class="container">
  <div class="item">Елемент 1</div>
  <div class="item">Елемент 2</div>
  <div class="item">Елемент 3</div>
</div>
```
CSS
```
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.item {
  width: 100px;
  height: 100px;
  background-color: red;
}
```
Този код ще подреди елементите в една колона, като центрира всеки елемент хоризонтално и вертикално.

CSS свойството **flex** се използва във Flexbox модела за управление на размерите на гъвкавите контейнери и техните деца. Кодът **flex: 1 1 auto;** задава стойности за следните параметри:

1. **flex-grow:** Определя се стойността на увеличението на елемента, когато има свободно пространство. В този случай, **flex-grow** е зададен на **1**, което означава, че елементът ще се разширява, ако има свободно пространство.
---
2. **flex-shrink:** Определя се стойността на смалението на елемента, когато няма достатъчно място. В този случай, **flex-shrink** също е зададен на **1**, което означава, че елементът може да се смали, ако няма достатъчно пространство.
---
3. **flex-basis:** Определя се началната размерна стойност на елемента преди да се приложат **flex-grow** и **flex-shrink**. За този случай, стойността е auto, която означава, че браузърът ще определи началния размер на елемента автоматично.

Комбинацията от **flex-grow**, **flex-shrink** и **flex-basis** позволява на елемента да се приспособи към различни размери на контейнера, като запазва съотношението на размерите си спрямо другите елементи във Flexbox контейнера.

---
Когато искаме да правим layout казваме **display: flex** като това трябва да го кажем на родителя(контейнера) на елементите, които искаме да подреждаме. Когато работим с flexbox имаме 2 основни групи от елементи. Имаме 1 елемент, който е нашият flex container, на който сме задали **display: flex**, и след това имаме flex items, или това са всичките деца (не наследници) на този елемент.

**Flexbox е мощен инструмент, който може да се използва за създаване на разнообразни оформления на елементи.**

---

## 06.Responsive Web Design

1. **Какво е Responsive Web Design?**
  - Responsive web design (RWD) е подход за създаване на уебсайтове, които автоматично се приспособяват към различните размери на екрана и устройствата, на които се визуализират, като например компютри, таблети и мобилни телефони.
  - Един уебсайт с responsive design ще се покаже по различен начин на големи десктоп екрани, в сравнение с по-малки екрани на мобилни устройства. Например, менюта могат да се преорганизират, изображенията да се смалят и текстът да се преформатира, за да се побере на по-тесни екрани.

2. **Защо е важен?**
 -  Responsive web design е важен, защото осигурява добро потребителско изживяване на всички устройства, които използват потребителите за достъп до уебсайтовете. Това подобрява удовлетвореността на потребителите, повишава достъпността и намалява отказите от уебсайтове.
 -  Без responsive design, уебсайтовете биха изглеждали некомфортно или невъзможно за използване на малки екрани, което би навредило на потребителското изживяване и би влошило репутацията на сайта.

3. **Какво е Mobile First и защо го използваме?**
 - Mobile First е подход в уеб дизайна, където се започва със създаването на уебсайтове за мобилни устройства и после се разширява функционалността за по-големите устройства. Този подход помага да се осигури по-добро приспособяване към мобилните потребители и по-добра производителност.
 - Започването със създаване на мобилна версия на уебсайта позволява на дизайнерите да се фокусират върху важните елементи и функционалности, които са необходими за мобилното изживяване. По този начин се осигурява по-ефективен и по-достъпен дизайн за потребителите с мобилни устройства.

4. **Какво са Media Queries?**
 - Media queries са CSS техника, която позволява на уеб дизайнерите да прилагат различни стилове в зависимост от характеристиките на устройството, като широчина на екрана, височина, разделителна способност и други.
 - Ето как изглеждат media queries в CSS:
```
@media screen and (max-width: 768px) {
    /* Стилове, които се прилагат при ширина на екрана до 768px */
}

@media (orientation: landscape) {
    /* Стилове, които се прилагат в хоризонтална ориентация */
}
```
---

## 07.Working with Forms

**01.What are Forms and How do we Use Them?**
- Формите в уеб разработката са интерактивни елементи, които позволяват на потребителите да въвеждат и предават информация към уеб приложенията. Те се използват за събиране на данни от потребителите, като например регистрационни форми, форми за вход, контактни форми и други, които се използват за комуникация и взаимодействие с потребителите на уебсайта.

Примерен HTML код:

```
<form action="/submit_form" method="POST">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>

  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required>

  <input type="submit" value="Submit">
</form>
```
**02.Styling a Form.**
- Стилизирането на форми се постига чрез CSS, което позволява на дизайнера да променя външния вид на формите, като прилага различни цветове, шрифтове, размери, бордюри и други стилове.

Примерен CSS код за стилизиране на форма:

```
form {
  background-color: #f2f2f2;
  padding: 20px;
  border-radius: 5px;
}

input[type="text"], input[type="password"] {
  width: 100%;
  padding: 10px;
  margin: 5px 0;
  border: 1px solid #ccc;
  border-radius: 4px;
}

input[type="submit"] {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type="submit"]:hover {
  background-color: #45a049;
}
```

**03.Responsive Forms with Flexbox**
- За да направим формите Responsive с Flexbox можем да използваме гъвкави контейнери.

Примерен CSS код за стилизиране на респонсивна форма с Flexbox:

```
form {
  display: flex;
  flex-direction: column;
  max-width: 400px;
  margin: auto;
  padding: 20px;
}

label {
  margin-bottom: 10px;
}

input[type="text"],
input[type="password"],
select,
textarea {
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

input[type="submit"] {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type="submit"]:hover {
  background-color: #45a049;
}
```
**04.Advanced Styling**
- За да приложим по-сложни стилове към формите, можем да използваме напреднали CSS техники като псевдокласове, псевдоелементи и CSS градиенти.

Примерен CSS код за напредно стилизиране на форми:

```
form {
  background-color: #f9f9f9;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

label {
  display: block;
  margin-bottom: 10px;
  font-weight: bold;
}

input[type="text"],
input[type="password"],
select,
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

input[type="submit"] {
  background: linear-gradient(to bottom, #4CAF50, #45a049);
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

input[type="submit"]:hover {
  background: linear-gradient(to bottom, #45a049, #4CAF50);
}
```





