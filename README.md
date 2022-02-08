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
USE sql_store;
SELECT * FROM customers;
SELeCT first_name, last_name FROM customers;
```

## Select data with Condition

```sql
SELECT * FROM customers WHERE customer_id=1;
```
