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

## Updating the values of a specific column in a table
## the syntax below is used

UPDATE `universitydb`.`students` SET `GPA` = '3.5' WHERE (`StudentID` = '1');
UPDATE `universitydb`.`students` SET `GPA` = '2.0' WHERE (`StudentID` = '2');
UPDATE `universitydb`.`students` SET `GPA` = '4.0' WHERE (`StudentID` = '3');
UPDATE `universitydb`.`students` SET `GPA` = '3.9' WHERE (`StudentID` = '4');
UPDATE `universitydb`.`students` SET `GPA` = '2.0' WHERE (`StudentID` = '5');

