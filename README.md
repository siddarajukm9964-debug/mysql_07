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


<!-- -- 1. Use LIKE to find all Customers whose names start with 'B'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE 'B%';

<!-- -- 2. Find all Customers whose names end with the letter 's'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE '%s';

<!-- -- 3. Find all Customers whose names contain the string 'on'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE '%on%';

<!-- -- 4. Use IN to select customers from multiple countries. -->
SELECT * FROM Customers
WHERE Country IN ('Germany', 'France', 'UK');

<!-- -- 5. Use BETWEEN to find products within a specific price range. -->
SELECT * FROM Products
WHERE Price BETWEEN 20 AND 50;

<!-- -- 6. Use NOT BETWEEN to find products outside a specific price range. -->
SELECT * FROM Products
WHERE Price NOT BETWEEN 20 AND 50;

<!-- -- 7. Use the AND operator to combine two conditions. -->
SELECT * FROM Customers
WHERE Country = 'Germany' AND City = 'Berlin';

<!-- -- 8. Use the OR operator to combine two conditions. -->
SELECT * FROM Customers
WHERE City = 'London' OR City = 'Paris';

<!-- -- 9. Use the NOT operator to exclude a condition. -->
SELECT * FROM Customers
WHERE NOT Country = 'USA';

<!-- -- 10. Use IS NULL to find records with missing values. -->
SELECT * FROM Orders
WHERE ShippedDate IS NULL;

<!-- -- 11. Use IS NOT NULL to find records that have values. -->
SELECT * FROM Orders
WHERE ShippedDate IS NOT NULL;

<!-- -- 12. Use the >= operator to filter data. -->
SELECT * FROM Products
WHERE Price >= 100;

<!-- -- 13. Use the <> operator to filter data. -->
SELECT * FROM Customers
WHERE Country <> 'UK';

<!-- -- 14. Find all Orders placed between two specific dates. -->
SELECT * FROM Orders
WHERE OrderDate BETWEEN '2023-01-01' AND '2023-12-31';

<!-- -- 15. Find all Products where the price is > 100 AND CategoryID is 2. -->
SELECT * FROM Products
WHERE Price > 100 AND CategoryID = 2;

<!-- -- 16. Find all Customers from 'London' OR 'Paris'. -->
SELECT * FROM Customers
WHERE City = 'London' OR City = 'Paris';

<!-- -- 17. Find all Employees who are NOT from the 'USA'. -->
SELECT * FROM Employees
WHERE Country <> 'USA';

<!-- -- 18. Find all Orders shipped after a specific date. -->
SELECT * FROM Orders
WHERE ShippedDate > '2023-01-01';

<!-- -- 19. Find all Products where the price is NOT between 20 and 50. -->
SELECT * FROM Products
WHERE Price NOT BETWEEN 20 AND 50;

<!-- -- 20. Combine LIKE and AND in a single query. -->
SELECT * FROM Customers
WHERE CustomerName LIKE 'A%' AND City = 'London';






<!-- -- 1. Use LIKE to find all Customers whose names start with 'B'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE 'B%';

<!-- -- 2. Find all Customers whose names end with the letter 's'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE '%s';

<!-- -- 3. Find all Customers whose names contain the string 'on'. -->
SELECT * FROM Customers
WHERE CustomerName LIKE '%on%';

<!-- -- 4. Use IN to select customers from multiple countries. -->
SELECT * FROM Customers
WHERE Country IN ('Germany', 'France', 'UK');

<!-- -- 5. Use BETWEEN to find products within a specific price range. -->
SELECT * FROM Products
WHERE Price BETWEEN 20 AND 50;

<!-- -- 6. Use NOT BETWEEN to find products outside a specific price range. -->
SELECT * FROM Products
WHERE Price NOT BETWEEN 20 AND 50;

<!-- -- 7. Use the AND operator to combine two conditions. -->
SELECT * FROM Customers
WHERE Country = 'Germany' AND City = 'Berlin';

<!-- -- 8. Use the OR operator to combine two conditions. -->
SELECT * FROM Customers
WHERE City = 'London' OR City = 'Paris';

<!-- -- 9. Use the NOT operator to exclude a condition. -->
SELECT * FROM Customers
WHERE NOT Country = 'USA';

<!-- -- 10. Use IS NULL to find records with missing values. -->
SELECT * FROM Orders
WHERE ShippedDate IS NULL;

<!-- -- 11. Use IS NOT NULL to find records that have values. -->
SELECT * FROM Orders
WHERE ShippedDate IS NOT NULL;

<!-- -- 12. Use the >= operator to filter data. -->
SELECT * FROM Products
WHERE Price >= 100;

<!-- -- 13. Use the <> operator to filter data. -->
SELECT * FROM Customers
WHERE Country <> 'UK';

<!-- -- 14. Find all Orders placed between two specific dates. -->
SELECT * FROM Orders
WHERE OrderDate BETWEEN '2023-01-01' AND '2023-12-31';

<!-- -- 15. Find all Products where the price is > 100 AND CategoryID is 2. -->
SELECT * FROM Products
WHERE Price > 100 AND CategoryID = 2;

<!-- -- 16. Find all Customers from 'London' OR 'Paris'. -->
SELECT * FROM Customers
WHERE City = 'London' OR City = 'Paris';

<!-- -- 17. Find all Employees who are NOT from the 'USA'. -->
SELECT * FROM Employees
WHERE Country <> 'USA';

<!-- -- 18. Find all Orders shipped after a specific date. -->
SELECT * FROM Orders
WHERE ShippedDate > '2023-01-01';

<!-- -- 19. Find all Products where the price is NOT between 20 and 50. -->
SELECT * FROM Products
WHERE Price NOT BETWEEN 20 AND 50;

<!-- -- 20. Combine LIKE and AND in a single query. -->
SELECT * FROM Customers
 WHERE CustomerName LIKE 'A%' AND City = 'London';