# MySQL #

### SELECT ###
The SELECT statement is used to select data from a database

```sql
SELECT column1, column2, ... FROM table_name;
```

Used to select all columns
```sql
SELECT * FROM table_name;
```

Used to return only distinct (different) values
```sql
SELECT DISTINCT column1, column2, ... FROM table_name;
```

### WHERE ###
The WHERE clause is used to filter records

```sql
SELECT column1, column2, ... FROM table_name WHERE condition;
```

Equal
```sql
SELECT * FROM Customers WHERE Country = 'Mexico';
SELECT * FROM Customers WHERE CustomerID = 1;
```

Greater than
```sql
SELECT * FROM Products WHERE Price > 30;
```

Less than
```sql
SELECT * FROM Products WHERE Price < 30;
```

Greater than or equal
```sql
SELECT * FROM Products WHERE Price >= 30;
```

Less than or equal
```sql
SELECT * FROM Products WHERE Price <= 30;
```

Not equal
```sql
SELECT * FROM Products WHERE Price <> 30;
```

Between a certain page
```sql
SELECT * FROM Product WHERE Price BETWEEN 50 AND 60;
```

Search for a pattern
```sql
SELECT * FROM Customers WHERE City LIKE 's%';
```

To specify multiple possible values for a column
```sql
SELECT * FROM Customers WHERE City IN ('Paris','London');
```

### AND, OR, NOT ###
The AND operator displays a record if all the conditions separated by AND are TRUE
```sql
SELECT column1, column2, ... FROM table_name WHERE condition1 AND condition2 AND condition3 ...;
SELECT * FROM Customers WHERE Country = 'Germany' AND City = 'Berlin';
```

The OR operator displays a record if any of the conditions separated by OR is TRUE
```sql
SELECT column1, column2, ... FROM table_name WHERE condition1 OR condition2 OR condition3 ...;
SELECT * FROM Customers WHERE Country = 'Germany' OR City = 'Berlin';
```

The NOT operator displays a record if the condition(s) is NOT TRUE
```sql
SELECT column1, column2, ... FROM table_name WHERE NOT condition;
SELECT * FROM Customers WHERE NOT Country = 'Germany';
```

