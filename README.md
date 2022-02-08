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
```
