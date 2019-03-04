###Задача

Допустим, мы собираем внутреннюю библиотеку книг по программированию, поэтому хотим иметь приложение, которое бы показывало все книжные новинки.
Приложение периодически собирает данные с одного или нескольких интернет-магазинов и показывает в удобной нам форме.

Источником данных является магазин издательства "Питер" или любой аналогичный магазин, на выбор исполнителя:
https://www.piter.com/collection/biblioteka-programmista
Требования к загрузке данных:
- данные должны обновляться периодически (раз в сутки);
- книги при обновлении не должны дублироваться;
- должна быть учтена возможность одновременного подключения нескольких источников данных.
Реализация работы с множественными источниками не требуется, но должна быть учтена в архитектуре приложения.

Для отображения данных необходимо сделать страницу с поиском (ЧПУ страницы любое). 
Страница содержит таблицу со следующими полями: название книги, год издания, изображение, автор (авторы), стоимость.
Таблица отображает книги по 10 штук, если их больше, необходимо сделать пагинацию.
Форма поиска содержит одно поле ввода и позволяет искать одновременно по автору и/или названию книги.
Визуальное представление страницы на выбор исполнителя.

Для хранения книг используется MySQL. Структура таблицы/таблиц на выбор исполнителя. При построении структуры необходимо учитывать, что книг может быть много (тысячи).


Данные: Книги (название, год издания, изображение, автор/авторы, стоимость).
Внешний источник: https://www.piter.com/collection/biblioteka-programmista или аналогичный.
База данных: MySQL (актуальная версия)
Фреймворк: Laravel (актуальная версия)
Дополнительная информация, которая может быть полезной в решении: https://github.com/dweidner/laravel-goutte
Примерное время выполнения: 3 часа.