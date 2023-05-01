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
## **SELECT * FROM orders WHERE status != "cancelled"**
#
## 8)Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
## Вывести нужно только номер (id) и сумму (sum) заказа.
## **SELECT id, sum FROM orders WHERE products_count > 3**
#
## 9) Выберите из таблицы orders все отмененные заказы. У отмененных заказов status равен "cancelled".
## **SELECT * FROM orders WHERE status = "cancelled"**
# 
## 10)  Выберите из таблицы orders все отмененные (cancelled) и возвращенные (returned) товары.
## Используйте IN.
## 1 - решение **SELECT * FROM orders WHERE status IN ("cancelled", "returned")**
## 2 - решение **SELECT * FROM orders WHERE status = "cancelled" OR status = "returned**
#
## 11) Выберите из таблицы orders все заказы, у которых сумма (sum) больше 3000 или количество товаров (products_count) от 3 и больше.
## **SELECT * FROM orders WHERE sum > 3000 OR products_count >= 3**
#
## 12) Выберите из таблицы orders все отмененные заказы стоимостью от 3000 до 10000 рублей включительно. Используйте BETWEEN.
## **SELECT * FROM orders WHERE status = "cancelled" and sum >= 3000 and sum <= 10000**
#
## 13) Выберите из таблицы orders все отмененные заказы исключая заказы стоимостью от 3000 до 10000 рублей включительно.
## **SELECT * FROM orders WHERE (status = "cancelled") AND (sum < 3000 OR sum > 10000)**
#
## 14) Выберите из таблицы products все товары в порядке возрастания цены (price).
## **SELECT * FROM products ORDER BY (для сортировки) price**
#
## 15) Выберите из таблицы products все товары в порядке убывания цены.
## Выведите только имена (name) и цены (price).
## **SELECT name, price FROM products ORDER BY price DESC**
#
## 16) Выберите из таблицы products все товары стоимостью 5000 и выше в порядке убывания цены (price).
## **SELECT * FROM products WHERE price >= 5000 ORDER BY price DESC** (DESC - сортирует в обратном порядке)
#
## 17) Выберите из таблицы products все товары стоимостью до 3000 рублей отсортированные в алфавитном порядке. Вывести нужно только имя (name), количество (count) и цену (price).
## **SELECT name, count, price FROM products**
## **WHERE price < 3000** (вывод нужного значения)
## **ORDER BY name** (Сортировка)
# 
## 18)