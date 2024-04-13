CREATE TABLE dishes(
dishID INT UNIQUE,
dishName VARCHAR (50),
orderID INT
);

# Add a foreignKey constraint

ALTER TABLE dishes
ADD CONSTRAINT FK_orderID
FOREIGN KEY (OrderID)
REFERENCES orders(orderID);

# adding Unique contraint to an existing table

ALTER TABLE customer
ADD CONSTRAINT UC_CustomerNumber UNIQUE (CustomerID);

# dropping the unique constraint

ALTER TABLE customer
DROP CONSTRAINT UC_CustomerNumber;

ALTER TABLE customer
ADD CONSTRAINT UC_CustomerNumber UNIQUE (CustomerNumber);

