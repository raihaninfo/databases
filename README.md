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
