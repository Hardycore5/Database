## Schema Design

A database schema is the blueprint of a database.
Just like an architect draws a plan before building a house,
a developer designs a schema before building a database.

The schema defines:
- What tables exist in the database
- What columns each table has
- What data type each column stores
- How tables are connected to each other

A well-designed schema makes a database reliable, 
efficient, and easy to work with. A poorly designed 
schema causes problems that are very hard to fix later.

## What a Schema Includes

A database schema is made up of several key components:

1. Tables — the main structures that hold the data
2. Columns — the specific categories of data in each table
3. Data Types — the rules for what kind of data each column stores
4. Constraints — rules that protect the accuracy of the data
5. Relationships — the connections between different tables

Example schema for a school database:
- Students table: id, name, age, class_id
- Classes table: id, class_name, teacher_name
- The class_id in Students connects to the id in Classes

## What is Normalization?
Normalization is the process of organizing a database 
to reduce unnecessary repetition of data.

Imagine writing every student's class name in full 
on every single row — "Primary Five East" repeated 
500 times. That wastes space and causes problems 
if the class name ever changes!

Normalization solves this by:
- Removing repeated data
- Storing each piece of information in only one place
- Connecting tables through keys instead of repeating values

A normalized database is cleaner, smaller, 
and much easier to maintain.
