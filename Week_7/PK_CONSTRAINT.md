CREATE DATABASE hospital;

USE hospital;

CREATE TABLE Pharmacy(
pharmacyID INT PRIMARY KEY,
pharmacyName VARCHAR (50)
);

# Drop primary key

ALTER TABLE pharmacy
DROP PRIMARY KEY

# Add primary Key to the pharmacy table using the alter syntax

ALTER TABLE pharmacy
ADD PRIMARY KEY (pharmacyID)
