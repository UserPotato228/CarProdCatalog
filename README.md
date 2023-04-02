# CarProdCatalog - Репозиторий для дисциплины ТРЗБД
В данном репозитории находятся диаграмма для БД **CarProdCatalog** 
>CarProdCatalog/ERD.drawio

Так же запросы по созданию таблиц, записей в БД
>CarProdCatalog/ComingSoon.frmt

>CarProdCatalog/ComingSoon.frmt

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
* **Desc** `text` `NOT NULL`
* **Rack** `int` `NOT NULL`
* **Column** `int` `NOT NULL`
* **Row** `int` `NOT NULL`

Где 
* ID - ИН товара
* ID_category - ИН категории
* Amount - Кол-во товара
* Cost - Стоимость
* Code - Артикул
* Desc - Описание/Характеристики
* Rack - Стелаж
* Column - Ряд
* Row - Полка

В **Categories**
* `PK` **ID** `serial\autoincrement` 
* **Name** `varchar(100)` `NOT NULL`

Где 
* ID - ИН категории
* Name - Наименование

В **Orders**
* `PK` **ID** `serial\autoincrement`
* `FK > Products.ID` **ID_product** `int` `NOT NULL`
* `FK > Customers.ID` **ID_customer** `int` `NOT NULL`
* **Order_date** `date` `NOT NULL`

Где 
* ID - ИН заказа
* ID_product - ИН товара
* ID_customer - ИН заказчика
* Order_date - Дата заказа

В **Customers**
* `PK` **ID** `serail\autoincrement`
* **Full_name** `nvarhar(100)` `NOT NULL` 
* **Phone_num** `int` `NOT NULL`

Где 
* ID - ИН заказчика
* Full_name - ФИО
* Phone_num - Номер телефона

### foooter
 $$${\color{gray}Masunya \space will \space be \space no \space more}$$$
