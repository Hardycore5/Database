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

## SQL Clauses and JOIN Types

**INNER JOIN**
Returns only the rows where there is a matching value 
in both tables being joined.

**LEFT JOIN**
Returns all rows from the left table, and matching rows 
from the right table. Non-matching rows show NULL.

**WHERE Clause**
Used to filter query results — showing only rows 
that meet a specific condition.

**ORDER BY**
Used to sort query results in ascending (ASC) 
or descending (DESC) order.

**LIMIT**
Used to restrict the number of rows returned 
by a SELECT query.

## Data Types

**Data Type**
A rule that defines what kind of information can be 
stored in a specific column of a table.

**VARCHAR**
A data type for storing short text — like names or titles.
Example: name VARCHAR(100)

**INTEGER**
A data type for storing whole numbers.
Example: age INTEGER

**BOOLEAN**
A data type that stores only TRUE or FALSE.
Example: is_enrolled BOOLEAN

**DATE**
A data type for storing dates in YYYY-MM-DD format.
Example: birthday DATE

## Database Design Terms

**Record**
Another word for a row — a single complete entry in a table.

**Field**
Another word for a column — a specific category of data.

**Constraint**
A rule applied to a column to protect data accuracy.
Example: NOT NULL means a column cannot be left empty.

**Redundancy**
When the same data is stored in more than one place 
unnecessarily. Normalization helps remove redundancy.

**Data Integrity**
The accuracy and consistency of data stored in a database.
Good schema design and constraints protect data integrity.

## Additional Design Terms

**Attribute**
A property or characteristic of an entity. 
In a table, each column represents an attribute.

**Entity**
A real-world object or concept represented as a table.
Example: Student, Class, and Teacher are all entities.

**Relationship**
A connection between two entities (tables) in a database.

**Tuple**
A formal word for a row or record in a table.

**Cardinality**
Describes how many instances of one entity relate 
to instances of another.
Example: One teacher can have MANY students.

## Advanced Terms

**ACID**
Four properties that guarantee reliable transactions:
Atomicity, Consistency, Isolation, Durability.

**Transaction**
A sequence of SQL operations treated as one unit.
Either ALL succeed or NONE of them do.

**Stored Procedure**
A saved set of SQL commands that can be reused.

**View**
A virtual table created from a SELECT query.

**Backup**
A saved copy of the database for recovery purposes.

## Transaction and ACID Definitions

**ACID Compliance**
When a database fully supports all four ACID properties.
Most relational databases like MySQL are ACID compliant.

**Atomicity**
The guarantee that a transaction is all or nothing.

**Consistency**
The guarantee that a transaction keeps the database valid.

**Isolation**
The guarantee that transactions do not interfere 
with each other.

**Durability**
The guarantee that completed transactions are 
saved permanently.
