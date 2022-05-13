
1. Какие есть способы объявления функций?   
> Function Declaration (основной)
> Function Expression
> Стрелочные функции (самый новый)
2. Приведите примеры вызова одной и той же функции всеми известными вам способами.
function sayOne() {       
  alert( "Один" );
}
let sayTwo = function() {  
  alert( "Два" );
};
let sayThree = () => alert("Три!");
3. В чем разница между тестированием и отладкой (дебаггингом)? А что такое логирование

4. В чем разница между Function Expression и Function Declaration? 
**Function Declaration**
 – функция, объявленная в основном потоке кода. 
**Function Expression**
 – объявление функции в контексте какого-либо выражения, например присваивания

5. Что делает функция `console.log()`? 
Метод console.log() выводит отладочную информацию в консоль, т.е. скрывая ее от пользователей.

6. Что такое BOM и DOM? 
BOM (модель объекта браузера) состоит из объектов `navigator`
, `history`
, `screen`
, `location`
 и `document`
, которые являются дочерними элементами `window`
. В `document` node находится DOM (Document Object Model), объектная модель документа, которая представляет содержимое страницы. Вы можете манипулировать им с помощью javascript.

7 Есть вот такая страница:
    Как найти в ней?…
1. Таблицу с `id="age-table"`

2. Все элементы `label` внутри этой таблицы (их три)

document.getElementsByTagName('label')[0].value = 3;

3. Форму `form` с именем `name="search"`
  let inputs = table.getElementsByTagName('form');
	console.log(inputs);
8.  Как сделать переход на другую страницу при клике на кнопку (без `<a href=...>`, только средствами JavaScript)?  
`document.location.href = "http://www.site.ru";`

9. Как можно обнулить (очистить) значение внутри input?  

10. Как будет выглядеть ваша функция приветствия из прошлого домашнего задания, если ее переписать в стрелочном формате?

let name = ("Как тебя зовут?") => message_to (`Привет ${name}`);
message_to();