# SQL Practice Exercises

## Database Schema
### Tables Structure
1. **Customers**
   - CustomerID
   - CustomerName
   - ContactName
   - Country

2. **Orders**
   - OrderID
   - CustomerID
   - OrderDate

3. **Products**
   - ProductID
   - ProductName
   - Price
   - CategoryID

4. **Categories**
   - CategoryID
   - CategoryName

5. **Employees**
   - EmployeeID
   - LastName
   - FirstName
   - BirthDate

## Exercises with Solutions

### 1. Basic SELECT Query
Find all customers from Germany
```sql
-- Your solution here:

-- Solution (hover or select to reveal):
SELECT * 
FROM Customers 
WHERE Country = 'Germany';
```

### 2. JOIN Practice
Get all orders made by customer 'Around the Horn' including order dates
```sql
-- Your solution here:

```

### 3. Aggregate Functions
Count the number of customers in each country
```sql
-- Your solution here:

```

### 4. Advanced Query
Find the top 3 most ordered products
```sql
-- Your solution here:

-- Solution (hover or select to reveal):

```

---

Would you like to:
- Try these exercises?
- Get more exercises?
- Focus on a specific SQL concept?
- Get explanations for any of the solutions?

<div style="color: white; background: white;">
Note: The solutions above use the following concepts:
- Basic SELECT with WHERE clause
- INNER JOIN between tables
- Aggregate functions (COUNT)
- GROUP BY and ORDER BY
- LIMIT clause
- Multiple table joins
</div>