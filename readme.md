# Ion.Calendar
Удобный легкий календарь <a href="http://ionden.com/a/plugins/ion.calendar/">Страница проекта</a>

***

## Описание
ion.calendar — красивый, удобный и легко настраиваемый календарь, основанный на мощной библиотеке для работы со временем "Moment.js". Календарь поддерживает разнообразные события и может работать как datepicker. Кроме того внешний вид календаря полностью настраивается через CSS.
Календарь лишен избыточных элементов управления. Стрелочки влево/вправо переключают месяц. Клик по текущей дате, позволяет выбрать другой год.
Календарь свободно распространяется на условиях <a href="http://ionden.com/a/licence.html">лицензии MIT</a>.

## Зависимости
* <a href="http://jquery.com/" target="_blank">jQuery 1.7.2+</a>
* <a href="http://momentjs.com/" target="_blank">Moment.js 1.7+</a>


## Подключение

Подключаем библиотеки:
* jQuery
* moment.min.js
* moment.ru.js
* ion.calendar.js

И CSS:
* ion.calendar.css

Инициализируем календарь:
<pre><code>$("#calendar_container").ionCalendar();</code></pre>

Или инициализируем календарь с параметрами:
<pre><code>$("#calendar_container").ionCalendar({
    lang: "ru",                     // язык календаря
    format: "LL",                   // формат возвращаемой даты
    onUpdate: function(date){       // callback функция, вызывается при каждой смене месяца
        console.log(date);
    },
    onClick: function(date){        // callback функция, вызывается при каждом клике по дню
        console.log(date);
    }
});
</code></pre>