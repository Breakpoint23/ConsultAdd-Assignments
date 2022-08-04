# Question1
SELECT DISTINCT City from customers;
SELECT COUNT(DISTINCT City) FROM customers;
Answer= 69.

# Question2
SELECT MIN(Quantity) as min_order,MAX(Quantity) as max_order FROM order_details;
Answer= 1, 120.

# Question3
SELECT SUM(Quantity) as Total,AVG(Quantity) as Average FROM order_details;
Answer=12743,24.6004

# Question4
SELECT ProductName from products LIMIT 4,10;

# Question5
SELECT * FROM suppliers WHERE SupplierName like '_a%';_

# Question6
SELECT * FROM customers WHERE Country!="USA" AND Country!="Canada";

# Question7
SELECT * FROM order_details WHERE OrderID in (SELECT OrderID FROM orders WHERE OrderDate>='2020-01-01' AND OrderDate<"2021-01-01");

# Question8
SELECT * FROM employees WHERE FirstName!="Sanjay" AND FirstName!="Sonia";

# Question9
CREATE TABLE SupplierDetail AS SELECT * FROM suppliers;

# Question10
DELETE FROM customers as c WHERE c.Country="Venezuela";
SELECT * FROM customers;
