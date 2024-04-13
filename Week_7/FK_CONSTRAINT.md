-- CREATE DATABASE hotel;
-- USE hotel;

-- CREATE TABLE Customer(
-- CustomerID INT PRIMARY KEY,
-- CustomerNumber INT,
-- CustomerName VARCHAR (50)
-- );

-- ALTER TABLE Customer
-- DROP PRIMARY KEY;

-- ALTER TABLE Customer
-- ADD PRIMARY KEY (CustomerID);


-- CREATE TABLE Orders(
-- OrderID INT PRIMARY KEY,
-- OrderNAme VARCHAR (50),
-- OrderDate Date
-- );

# add the CustomerID column to the orders table

-- ALTER TABLE orders
-- ADD CustomerID INT ;

# Adding a foreignKey Constraint

-- ALTER TABLE orders 
-- ADD CONSTRAINT FK_CustomerID
-- FOREIGN KEY (CustomerID)
-- REFERENCES Customer (CustomerID);

# Dropping a FK contraint

-- ALTER TABLE orders
-- DROP CONSTRAINT FK_CustomerID;

# add the FK contraint again

-- ALTER TABLE orders
-- ADD CONSTRAINT FK_CustomerID
-- FOREIGN KEY (CustomerID)
-- REFERENCES Customer (CustomerID);

