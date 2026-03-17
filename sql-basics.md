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
