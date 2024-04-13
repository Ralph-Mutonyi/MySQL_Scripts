ALTER TABLE customer
MODIFY CustomerName VARCHAR(50) NOT NULL;

# removing the not null constraint

ALTER TABLE customer
MODIFY CustomerName VARCHAR(50);
