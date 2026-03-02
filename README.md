<!-- -- 1. Select all columns from the Customers table. -->
SELECT * FROM Customers;

<!-- -- 2. Select only the CustomerName column from Customers. -->
SELECT CustomerName FROM Customers;

<!-- -- 3. Select distinct Country from the Customers table. -->
SELECT DISTINCT Country FROM Customers;

<!-- -- 4. Select the City column from the Customers table. -->
SELECT City FROM Customers;

<!-- -- 5. Select all Products where the Price is greater than 50. -->
SELECT * FROM Products
WHERE Price > 50;

<!-- -- 6. Select all Orders where the OrderID is exactly 10248. -->
SELECT * FROM Orders
WHERE OrderID = 10248;

<!-- -- 7. Select all Customers who live in 'Germany'. -->
SELECT * FROM Customers
WHERE Country = 'Germany';



<!-- -- 9. Select all Products where the CategoryID is 1. -->
SELECT * FROM Products
WHERE CategoryID = 1;

<!-- -- 10. Select the top 5 Customers. -->
SELECT TOP 5 * FROM Customers;   -- (SQL Server)

<!-- -- 11. Select the first 10 Products. -->
SELECT * FROM Products
LIMIT 10;   -- (MySQL / PostgreSQL)

<!-- -- 12. Select unique Cities from the Customers table. -->
SELECT DISTINCT City FROM Customers;

<!-- -- 13. Select all Orders where the ShipCountry is 'USA'. -->
SELECT * FROM Orders
WHERE ShipCountry = 'USA';

<!-- -- 14. Select all Customers whose CustomerID starts with the letter 'A'. -->
SELECT * FROM Customers
WHERE CustomerID LIKE 'A%';

<!-- -- 15. Select all Products with a price between 10 and 20. -->
SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20;

<!-- -- 16. Select all Orders where the OrderDate is NULL. -->
SELECT * FROM Orders
WHERE OrderDate IS NULL;

<!-- -- 17. Select all Employees whose LastName is 'Davolio'. -->
SELECT * FROM Employees
WHERE LastName = 'Davolio';

<!-- -- 18. Select all Products that are NOT in category 2. -->
SELECT * FROM Products
WHERE CategoryID <> 2;

<!-- -- 19. Select all Customers living in either 'Germany' or 'France'. -->
SELECT * FROM Customers
WHERE Country IN ('Germany', 'France');

<!-- -- 20. Select all Customers who are NOT from the 'UK'. -->
SELECT * FROM Customers
WHERE Country <> 'UK';



   
