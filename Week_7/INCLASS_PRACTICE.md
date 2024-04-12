CREATE DATABASE school;

USE school;

CREATE TABLE students (
	studentsID INT PRIMARY KEY,
    firstName	VARCHAR (50),
    LastName 	VARCHAR (50)
    );

# Alter Table - add a primary key to a table

ALTER TABLE students
ADD PRIMARY KEY (studentsID);

# a table cant have multiple primary keys

# remove primary key --> Drop column

ALTER TABLE students
DROP PRIMARY KEY;

ALTER TABLE students
ADD PRIMARY KEY (studentsID);

CREATE TABLE Customers(
CustomerID INT PRIMARY KEY,
CustomerName VARCHAR(50)
);

CREATE TABLE Orders(
OrderID INT PRIMARY KEY,
CustomerID INT,  -- foreign key 
OrderDate DATE
);

# adding a foreign key

ALTER TABLE Orders
ADD CONSTRAINT FK_CustomerID
FOREIGN KEY (CustomerID)
REFERENCES Customers (CustomerID);

# Dropping a foreign Key

ALTER TABLE Orders
DROP CONSTRAINT FK_CustomerID

# UNIQUE CONTRAINT