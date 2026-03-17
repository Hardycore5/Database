## Database Glossary

This file contains clear definitions for every key term 
encountered throughout this project.

Whenever you come across a word you are not sure about,
check here first. All definitions are written in 
plain, simple language.

The glossary grows with every new term learned —
making it a living reference that builds over time.

## Terms A-C

**Database**
An organized collection of information stored electronically,
managed by software called a DBMS.

**DBMS (Database Management System)**
The software that manages a database — allowing you to 
store, find, update, and delete information.
Examples: MySQL, PostgreSQL, SQLite.

**Table**
A structure inside a database that holds data organized 
into rows and columns — like a grid or spreadsheet.

**Row (Record)**
A single, complete entry in a table. 
Holds all the information about one specific thing.

**Column (Field)**
A specific category of data within a table.
Runs from top to bottom and stores one type of information.

## Terms P-S

**Primary Key**
A unique identifier for each row in a table.
No two rows can have the same primary key value.

**Foreign Key**
A column in one table that refers to the primary key 
in another table, creating a link between the two.

**Schema**
The blueprint or structure of a database — defining 
tables, columns, data types, and relationships.

**Query**
A request sent to a database asking it to retrieve, 
add, update, or delete information. Written in SQL.

**Index**
A structure that helps the database find information 
faster — like the index at the back of a textbook.

## Terms S-N

**SQL (Structured Query Language)**
The standard language used to communicate with 
a relational database.

**NoSQL**
A type of database that does not use traditional tables.
Stores data in flexible formats like documents or key-value pairs.

**Relational Database**
A database that organizes data into tables connected 
to each other through relationships using keys.

**Normalization**
The process of organizing a database to remove 
unnecessary repetition and improve data accuracy.

**NULL**
A special marker meaning a field has no value at all.
Not the same as zero or an empty string — it means 
the information is completely absent.

## Core SQL Commands

**SELECT**
The SQL command used to retrieve data from a table.
Example: SELECT name FROM students;

**INSERT INTO**
The SQL command used to add a new row into a table.
Example: INSERT INTO students (name, age) VALUES ('Emeka', 10);

**UPDATE**
The SQL command used to change existing data in a table.
Always use with WHERE to avoid changing every row.

**DELETE**
The SQL command used to permanently remove a row from a table.
Always use with WHERE to avoid deleting everything.

**JOIN**
A SQL operation that combines rows from two or more tables 
based on a shared column between them.
