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
```
