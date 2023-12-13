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

### **Comparison Operators in WHERE Clause:**
  
Comparison operators (e.g., =, <>, >, <, >=, <=) are used to compare values in the WHERE clause. For example, to retrieve products with a unit price less than 50, you can use the following query:

```sql
SELECT product_name, unit_price FROM products WHERE unit_price < 50;
```

### **Using Wildcards with WHERE Clause:**
The WHERE clause can also be used with wildcard characters for pattern matching. For instance, to retrieve all customers with names starting with "Joh," you can use the LIKE operator and the '%' wildcard as follows:

```sql
SELECT * FROM customers WHERE customer_name LIKE 'Joh%';  
 ```

### **Combining Conditions with Parentheses:**
To create more complex conditions, you can use parentheses to group logical expressions. For example, to retrieve products with a unit price less than 50 or belonging to the "Electronics" category, you can use parentheses and the OR operator as follows:

```sql
SELECT product_name, unit_price, category FROM products WHERE (unit_price < 50 OR category = 'Electronics');  
```

### **NULL Values and IS NULL/IS NOT NULL:**
To filter rows based on **NULL** values, you can use the **IS NULL** or **IS NOT NULL** operators. For example, to retrieve employees with no assigned manager, you can use the following query:

```sql
SELECT * FROM employees WHERE manager_id IS NULL;
```
