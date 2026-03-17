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

## First Normal Form (1NF)
The first rule of normalization is called First Normal Form.

A table is in First Normal Form when:
1. Every column contains only one single value per row
2. Every row is unique — no two rows are exactly the same
3. Each column has a clear and consistent data type

Example of BREAKING 1NF:
| Name  | Subjects                |
|-------|-------------------------|
| Emeka | Maths, English, Science |

Example of FOLLOWING 1NF:
| Name  | Subject |
|-------|---------|
| Emeka | Maths   |
| Emeka | English |
| Emeka | Science |

Each box contains only one value — clean and organized!

## Second Normal Form (2NF)
A table is in Second Normal Form when:
1. It already follows First Normal Form (1NF)
2. Every non-key column depends on the WHOLE primary key
   — not just part of it

This mainly applies to tables that have a 
combined primary key (two columns together as the key).

Example:
If a table uses both Student ID and Subject as its key,
then every other column must depend on BOTH together —
not just one of them.

Achieving 2NF usually means splitting one large table 
into two smaller, more focused tables. This keeps 
each table responsible for only one thing.

## Third Normal Form (3NF)
A table is in Third Normal Form when:
1. It already follows Second Normal Form (2NF)
2. Every non-key column depends ONLY on the primary key

In simple terms — no column should depend on 
another non-key column. Every column must answer 
directly to the primary key alone.

Example of BREAKING 3NF:
If a Students table has a "City" column AND a 
"Country" column — Country depends on City, 
not on the Student ID. That breaks 3NF.

Fix: Move City and Country into their own separate table
and link it back using a key.

3NF produces the cleanest, most efficient database design.
