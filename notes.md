## What is a Database?
A database is an organized collection of information stored 
on a computer. Just like how a library stores books in a 
neat order so you can find them easily, a database stores 
information neatly so a computer can find it quickly.

This file is where I write down everything I learn about databases.
I will keep updating it as I go.

## Data vs Information
- Data is raw facts on their own. Example: "8", "John", "Nigeria"
- Information is when data is given meaning. Example: 
  "John is 8 years old and lives in Nigeria."
- Databases store data and help turn it into useful information.

- ## What is a DBMS?
A DBMS (Database Management System) is the software that 
manages a database. It lets you store, find, update, and 
delete information easily.

Examples of popular DBMS software:
- MySQL
- PostgreSQL
- SQLite

## What is a Table?
A table is how information is stored inside a database. 
It looks like a grid with rows going across and columns 
going down — just like a chart in school.

Example: A table called "Students" might have columns for 
Name, Age, and Class, with each student taking up one row.

## What is a Row?
A row (also called a record) is one complete entry in a table.
It holds all the information about one single thing.

Example: In a Students table, one row might be:
Name: Emeka | Age: 10 | Class: Grade 5
That entire line is one row.

## What is a Column?
A column (also called a field) is one specific category 
of information in a table. It goes from top to bottom.

Example: In a Students table, the "Age" column would show 
the age of every single student listed in the table.

## What is SQL?
SQL stands for Structured Query Language. It is the 
language used to communicate with a database.

Just like you use English to talk to people, you use 
SQL to talk to a database — to ask it for information, 
add new information, change it, or delete it.

## What is a Relational Database?
A relational database is a type of database that stores 
information in tables that are connected to each other.

Example: A "Students" table and a "Classes" table can be 
connected so you know which student belongs to which class.
This connection between tables is called a relationship.

## What is a Primary Key?
A primary key is a unique identifier for each row in a table.
It makes sure no two rows are exactly the same.

Example: In a Students table, each student might have a 

## What is a Foreign Key?
A foreign key is a column in one table that points to the 
primary key in another table. It is how two tables are connected.

Example: A "Report Cards" table might have a Student ID column.
That Student ID comes from the "Students" table — 
making it a foreign key that links the two tables together.
unique Student ID like 001, 002, 003.
No two students can share the same ID — that is the primary key.

## The SELECT Statement
SELECT is the SQL command used to retrieve (read) data 
from a database table.

## Breaking Down a SELECT Statement

SELECT name FROM students;

- SELECT — means "show me"
- name — is the column you want to see
- FROM — means "look inside this table"
- students — is the name of the table
- ; — the semicolon means "end of instruction"

So the full sentence in plain English is:
"Show me the name column from the students table."

It is like asking the database: "Show me this information."

Basic example:
SELECT name FROM students;
This asks the database to show all the names 
from the students table.

## What Does SELECT * Mean?
The * symbol in SQL means "everything" or "all columns."

Example:
SELECT * FROM students;

This means: "Show me ALL the information from 
the students table" — every single column.

It is useful when you want to see the full picture 
instead of just one column.

## The WHERE Clause
WHERE is used to filter results. Instead of showing 
everything, it shows only the rows that match a condition.

Example:
SELECT name FROM students WHERE age = 10;

In plain English: "Show me the names of only the 
students who are 10 years old."

Without WHERE — you get everything.
With WHERE — you get only what you need.

## The INSERT INTO Statement
INSERT INTO is the SQL command used to add a new record 
(row) into a table.

It is like telling the database: "Add this new entry."

Basic example:
INSERT INTO students (name, age) VALUES ('Emeka', 10);

This adds a new student called Emeka who is 10 years old 
into the students table.

## Breaking Down INSERT INTO

INSERT INTO students (name, age) VALUES ('Emeka', 10);

- INSERT INTO — means "add a new row into this table"
- students — is the name of the table
- (name, age) — these are the columns you are filling in
- VALUES — means "here is the information to put in"
- ('Emeka', 10) — Emeka goes into the name column, 
  10 goes into the age column
- ; — end of instruction

Plain English: "Add a new student called Emeka 
who is 10 years old into the students table."

## The UPDATE Statement
UPDATE is the SQL command used to change existing 
information inside a table.

It is like telling the database: "Go find this record 
and change this part of it."

Basic example:
UPDATE students SET age = 11 WHERE name = 'Emeka';

This finds Emeka in the students table and 
changes his age to 11.
## WARNING — Always Use WHERE With UPDATE!
If you use UPDATE without WHERE, the database will 
change EVERY single row in the table — not just the one you want.

DANGEROUS example:
UPDATE students SET age = 11;
This changes EVERYONE'S age to 11. Not good!

SAFE example:
UPDATE students SET age = 11 WHERE name = 'Emeka';
This changes ONLY Emeka's age. 

Always double check your WHERE clause before updating!

## What Are Data Types?
A data type tells a database column what kind of 
information it is allowed to store.

Just like how a "Name" box should only have letters 
and an "Age" box should only have numbers — 
data types set the rules for each column.

This makes sure the right kind of information 
always goes into the right place.

## Common SQL Data Types

- INTEGER — stores whole numbers. Example: age = 10
- VARCHAR — stores short text like names. Example: name = 'Emeka'
- TEXT — stores longer text like descriptions
- DATE — stores dates. Example: birthday = '2015-03-17'
- BOOLEAN — stores only TRUE or FALSE. 
  Example: is_enrolled = TRUE

Choosing the right data type for each column keeps 
your database clean and accurate.



