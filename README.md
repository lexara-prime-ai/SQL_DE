## SQL LIMIT clause
```sql
SELECT column FROM table_name
-- Limit number of rows to 10
LIMIT 10
```

## SQL OFFSET clause
```sql
SELECT column FROM table_name
-- Will return results starting from the specified offset value
OFFSET number_of_rows 
```

## SQL WHERE clause
The basic syntax of the SQL **WHERE** clause is as follows:
```sql
SELECT column1, column2, ... FROM table_name WHERE condition;
```
### **Logical Operators in WHERE Clause:**
  
You can use logical operators (**AND, OR, NOT**) to create more complex conditions in the WHERE clause. For instance, to retrieve employees with a salary greater than 50000 and belonging to the "Sales" department, you can use the AND operator as follows:

```sql
SELECT * FROM employees WHERE salary > 50000 AND department = 'Sales';
```
