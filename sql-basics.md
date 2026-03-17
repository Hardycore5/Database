## SQL Basics — Reference Guide

This file is a structured reference guide for all the 
fundamental SQL commands covered in this project.

Whenever you need to remember how a SQL command works,
come here first! Each command has a clear explanation 
and a plain English example.

## SELECT
Used to retrieve data from a table.

Syntax:
SELECT column_name FROM table_name;

Example:
SELECT name FROM students;

Plain English: "Show me all the names 
from the students table."

To select everything:
SELECT * FROM students;
This shows every single column in the table.

## WHERE
Used to filter results and show only rows 
that match a specific condition.

Syntax:
SELECT column_name FROM table_name WHERE condition;

Example:
SELECT name FROM students WHERE age = 10;

Plain English: "Show me only the names of 
students who are 10 years old."

Common comparison operators:
- =  means equal to
- >  means greater than
- <  means less than
- != means not equal to

## INSERT INTO
Used to add a brand new row into a table.

Syntax:
INSERT INTO table_name (column1, column2) 
VALUES (value1, value2);

Example:
INSERT INTO students (name, age) VALUES ('Emeka', 10);

Plain English: "Add a new student called Emeka 
who is 10 years old into the students table."

## UPDATE
Used to change existing information in a table.

Syntax:
UPDATE table_name SET column_name = new_value 
WHERE condition;

Example:
UPDATE students SET age = 11 WHERE name = 'Emeka';

Plain English: "Find Emeka in the students table 
and change his age to 11."

IMPORTANT: Always use WHERE with UPDATE!
Without WHERE, every single row in the table 
will be changed — not just the one you want.

## DELETE
Used to permanently remove a row from a table.

Syntax:
DELETE FROM table_name WHERE condition;

Example:
DELETE FROM students WHERE name = 'Emeka';

Plain English: "Remove Emeka from the students table."

IMPORTANT: Always use WHERE with DELETE!
Without WHERE, every single row in the table 
will be deleted forever — there is no undo button!

## ORDER BY
Used to sort the results of a SELECT query 
in ascending or descending order.

Syntax:
SELECT column_name FROM table_name ORDER BY column_name ASC;

Examples:
SELECT name FROM students ORDER BY name ASC;
This shows student names from A to Z.

SELECT name FROM students ORDER BY age DESC;
This shows students from oldest to youngest.

- ASC = ascending (smallest to biggest, A to Z)
- DESC = descending (biggest to smallest, Z to A)
