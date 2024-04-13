CREATE DATABASE myCompany;

USE mycompany;

CREATE TABLE products(
productID INT PRIMARY KEY,
product_name VARCHAR (255) NOT NULL,

# check price is always positive ( column check)
selling_price NUMERIC (10,2) CHECK (selling_price > 0), 

# check that the cost is also always positive
cost NUMERIC (10,2) CHECK (cost > 0), 

# table check constraint. Not limited to one column. 
CONSTRAINT valid_selling_price CHECK (selling_price > cost)  
);
