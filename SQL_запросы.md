## 1) Получите всю информацию о товарах из таблицы products.
## **SELEKT * FROM products**
#
## 2) Получите название (name) и цену (price) всех товаров из таблицы products.
## **SELECT name, price FROM products**
#
## 3) Выберите из таблицы products все записи, в которых цена (price) меньше 3000.
## **SELECT * FROM products WHERE price < 3000;**
#
## 4) Выберите из таблицы products имена (name) и цены (price) всех товаров, 
## стоимостью от 10 000 и выше.
## **SELECT name, price FROM products WHERE price >= 10000;**
#
## 5) Получите из таблицы products имена (name) товаров, которые закончились.
## **SELECT name FROM products WHERE count = 0;**
#
## 6) Выберите из таблицы products название (name) и цены (price) товаров, 
## стоимостью до 4000 включительно.
## **SELECT name, price FROM products WHERE price <= 4000;**
#
## 7) Выберите из таблицы orders все заказы кроме отмененных. У отмененных заказов status равен 
## "cancelled".
##