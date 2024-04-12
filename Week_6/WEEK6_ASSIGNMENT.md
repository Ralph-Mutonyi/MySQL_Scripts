CREATE DATABASE UniversityDB

## ensure you are in the right db using the "USE" Keyword

USE Universitydb;

##  create a table called students

CREATE TABLE students(
StudentID INT PRIMARY KEY,
FirstName VARCHAR(50),
LastName VARCHAR (50),
Age INT,
Major VARCHAR (50)
);

## inset atleast 5 records

INSERT INTO students (studentID, FirstName, LastName, Age, Major)
VALUES 
(1, "Ralph", "Mutonyi", 21, "pharmacy"),
(2, "owen", "wekesa", 18, "Law"),
(3, "Gloria", "Musyoka", 22, "Medicine"), 
(4, "Daisy", "Keragori", 24, "Bussines"),
(5, "Mary", "james", 22, "Pharmacy");

## add another column 

ALTER TABLE students
ADD GPA VARCHAR(2);

## change the datatype of GPA

ALTER TABLE students
MODIFY GPA int;

## values of the GPA was input on the table directly  . The syntax used :

UPDATE `universitydb`.`students` SET `GPA` = '3.5' WHERE (`StudentID` = '1');
UPDATE `universitydb`.`students` SET `GPA` = '2.0' WHERE (`StudentID` = '2');
UPDATE `universitydb`.`students` SET `GPA` = '4.0' WHERE (`StudentID` = '3');
UPDATE `universitydb`.`students` SET `GPA` = '3.9' WHERE (`StudentID` = '4');
UPDATE `universitydb`.`students` SET `GPA` = '2.0' WHERE (`StudentID` = '5');


## Rename the students table

RENAME TABLE students TO EnrolledStudents

## create a new table called Courses

CREATE TABLE courses(
CourseID INT PRIMARY KEY,
CourseName VARCHAR(100),
Instructor VARCHAR (100),
Credits INT
);

## insert sample data into the table


INSERT INTO courses (CourseID, CourseName, Instructor, Credits)
VALUES
(1, "Pharmacy", "Prof. Abuga", 80),
(2, "Medicine and Surgery", "Prof Muriithi", 84),
(3, "Dentistry", "Dr. Ombet", 83);


## Drop the table enrolled students

DROP TABLE enrolledstudents;

