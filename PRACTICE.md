## In_class_mySQL_Scripts

-- CREATE DATABASE SAFARICOM;

-- USE safaricom;
-- CREATE TABLE Employees(
-- EmployeeID INT PRIMARY KEY, 
-- FirstName VARCHAR(255),
-- LastName VARCHAR(255),
-- DepartmentID INT,
-- HireDate DATE
-- );

-- INPUT DATA INTO THE TABLE

-- Create table 2

-- CREATE TABLE Products(
-- ProductID INT PRIMARY KEY,
-- ProductName VARCHAR (255) NOT NULL,
-- CategoryID INT,
-- Price DECIMAL (10, 2),
-- StockQuantity INT CHECK (StockQuantity >= 0)
-- );

-- alter  ( adding a new column)

-- ALTER TABLE employees
-- ADD Email VARCHAR(50);


-- ALTER TABLE employees
-- ADD Salary DECIMAL (10, 2);

-- modify existing column. 

-- ALTER TABLE products
-- MODIFY Price INT ;

-- ALTER TABLE products
-- MODIFY Price DECIMAL(10, 2);

-- deleting a column

-- ALTER TABLE employees
-- DROP COLUMN email;

-- ALTER TABLE employees
-- DROP COLUMN salary;

-- CREATE TABLE Inventory(
-- InventoryID INT  PRIMARY KEY,
-- itemName VARCHAR(255)
-- );

## Dropping  a table

-- DROP TABLE inventory;    this command is non reversible. 