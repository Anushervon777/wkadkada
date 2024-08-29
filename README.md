![](https://javascripttoday.com/images/post/dates_hub0fcfad55bf24f5711bb96d869002247_170726_1400x0_resize_box_3.png)
# Что такое NewDate в js ?
**В JavaScript объект Date используется для работы с датами и временем. Чтобы создать новый объект Date, используется конструктор new Date(). Вот несколько способов создания объекта Date**
```js
const now = new Date();
console.log(now); // Выводит текущую дату и время
```

```js
const specificDate = new Date('2024-08-29T08:32:09');
console.log(specificDate); // Вывод: Thu Aug 29 2024 08:32:09 GMT+0000 (UTC)

```

```js
const dateComponents = new Date(2024, 7, 29, 8, 32, 9); // Месяцы нумеруются с 0 (0 = январь, 11 = декабрь)
console.log(dateComponents); // Вывод: Thu Aug 29 2024 08:32:09 GMT+0000 (UTC)

```

```js
const milliseconds = new Date(1693305129000); // Миллисекунды с 1 января 1970 года
console.log(milliseconds); // Выводит дату, соответствующую миллисекундам

```
# Методы для работы с датами
```js
const date = new Date();
console.log(date.getFullYear()); // Получить год
console.log(date.getMonth()); // Получить месяц (0-11)
console.log(date.getDate()); // Получить день месяца (1-31)
console.log(date.getHours()); // Получить часы (0-23)
console.log(date.getMinutes()); // Получить минуты (0-59)
console.log(date.getSeconds()); // Получить секунды (0-59)

```

```js
const date = new Date();
date.setFullYear(2025);
date.setMonth(11); // Декабрь
date.setDate(25);
console.log(date); // Вывод: Thu Dec 25 2025 ...
```

```js
const date = new Date();
console.log(date.toDateString()); // Вывод: Thu Aug 29 2024
console.log(date.toISOString()); // Вывод: 2024-08-29T08:32:09.000Z

```
