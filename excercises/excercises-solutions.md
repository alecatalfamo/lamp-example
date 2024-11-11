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

-- Solution (hover or select to reveal):
SELECT Orders.OrderID, Orders.OrderDate
FROM Orders
INNER JOIN Customers 
ON Orders.CustomerID = Customers.CustomerID
WHERE Customers.CustomerName = 'Around the Horn';
```

### 3. Aggregate Functions
Count the number of customers in each country
```sql
-- Your solution here:

-- Solution (hover or select to reveal):
SELECT Country, COUNT(*) as CustomerCount
FROM Customers
GROUP BY Country
ORDER BY CustomerCount DESC;
```

### 4. Advanced Query
Find the top 3 most ordered products
```sql
-- Your solution here:

-- Solution (hover or select to reveal):
SELECT 
    Products.ProductName,
    COUNT(OrderDetails.OrderID) as TimesOrdered
FROM Products
INNER JOIN OrderDetails 
    ON Products.ProductID = OrderDetails.ProductID
GROUP BY Products.ProductName
ORDER BY TimesOrdered DESC
LIMIT 3;
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