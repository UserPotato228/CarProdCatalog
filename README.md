# CarProdCatalog - Репозиторий для дисциплины ТРЗБД
В данном репозитории находятся диаграмма для БД **CarProdCatalog** 
>CarProdCatelog/ERD.drawio

Так же запросы по созданию таблиц, записей в БД
# Структура
В БД **CarProdCatalog** находятся следующие таблицы
* Products
* Categories
* Orders
* Customers

В **Products** существуют следующие столбцы
* `PK` **ID** `serial\autoincrement`
* `FK > Categories.ID` **ID_category** `int` `NOT NULL`
* **Amount** `int` `NOT NULL`
* **Cost** `int` `NOT NULL`
* **Code** `int` `NOT NULL`
* **Desc** `int` `NOT NULL`
* **Rack** `int` `NOT NULL`
* **Column** `int` `NOT NULL`
* **Row** `int` `NOT NULL` 
