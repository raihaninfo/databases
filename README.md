# databases

> CREATE DATABASE testDB2;

> DROP DATABASE testDB2;

> use testDB;

```sql
CREATE TABLE user (
    userID int,
    FirstName varchar(255),
    LastName varchar(255),
    Address varchar(255),
    City varchar(255)
);
```

## Select data

```sql
-- select database
USE sql_store;
-- select all data form customers
SELECT * FROM customers;
-- select first name and last name
SELECT first_name, last_name FROM customers;

-- mathematical logic
SELECT points, points +1 FROM customers; -- result 2273, 2274
SELECT points, points -1 FROM customers; -- result 2273, 2272
SELECT points, points *10+100 FROM customers; -- result 2273, 22830
```

## Select data with Condition

```sql
SELECT * FROM customers WHERE customer_id=1;
SELECT * FROM customers WHERE birth_date > '1990-01-01';
```

## AND, OR and NOT Operators

```sql
SELECT * FROM customers WHERE birth_date > '1990-01-01' AND points >1000;
SELECT * FROM customers WHERE birth_date > '1990-01-01' OR points >1000;
SELECT * FROM customers WHERE NOT birth_date > '1990-01-01';
-- Result:= show all customers points between 1000 to 3000
SELECT * FROM customers WHERE points >=1000 AND points <=3000;
-- BETWEEN operators
SELECT * FROM customers WHERE points BETWEEN 1000 AND 3000;
```

## LIKE Operator

```sql
-- LIKE operator use search for any string
SELECT * FROM customers WHERE last_name LIKE 'b%';
```

## REGEXP operator

> https://www.educba.com/sql-regexp/

> https://dataschool.com/how-to-teach-people-sql/how-regex-works-in-sql/

[REGEXP online practice](https://regex101.com/)

```sql
SELECT * FROM customers WHERE last_name REGEXP 'field|mac|rose';
SELECT * FROM customers WHERE last_name REGEXP '[gim]e'; -- ge, ie, me
```

## NULL operator

```sql
SELECT * FROM customers WHERE phone IS NULL;
SELECT * FROM customers WHERE phone IS NOT NULL;
```

## ORDER

```sql
SELECT * FROM customers ORDER BY first_name;
SELECT * FROM customers ORDER BY first_name DESC;
```

## LIMIT

```sql
SELECT * FROM customers LIMIT 3; -- show only 3 result

```

## Inner join

```sql
SELECT order_id, orders.customer_id, first_name, last_name FROM orders JOIN
customers ON orders.customer_id = customers.customer_id;
```
