## Project Summary

This file brings together the most important concepts 
learned throughout the entire Database learning project.

It serves as a final consolidated reference where 
everything covered across all files comes together 
in one clear overview.

By reading this summary, you will see how far the 
journey has come — from knowing nothing about databases 
to having a solid foundation that real developers use.

## What is a Database?
A database is an organized collection of information 
stored electronically and managed by a DBMS.

Key components:
- Tables — hold data in rows and columns
- Rows — each one is a complete single entry
- Columns — each one is a specific category of data
- Primary Keys — unique IDs that identify each row
- Foreign Keys — links that connect tables together
- Schema — the overall blueprint of the database

Databases power almost every app in the world — 
from WhatsApp storing messages to Instagram 
storing photos and followers.

## SQL — The Language of Databases
SQL is how you communicate with a relational database.

The four core operations:
- SELECT — retrieve data from a table
- INSERT INTO — add new data to a table
- UPDATE — change existing data in a table
- DELETE — remove data from a table

Essential clauses:
- WHERE — filter results by a condition
- ORDER BY — sort results ascending or descending
- LIMIT — restrict how many results are returned
- JOIN — combine rows from two or more tables

Most important rule:
Always use WHERE with UPDATE and DELETE!

## Types of Databases

Relational (SQL) Databases:
- Store data in structured tables connected through keys
- Best for organized, structured data
- Examples: MySQL, PostgreSQL, SQLite

Non-Relational (NoSQL) Databases:
- Store data in flexible formats
- Best for rapidly changing or unstructured data
- Examples: MongoDB, Redis, Firebase

The rule of thumb:
- Structured data with clear relationships — use SQL
- Flexible data that changes shape often — use NoSQL
Many real-world applications use both together.

## Schema Design and Normalization

A schema is the blueprint of your database.

Normalization removes unnecessary repetition:
- 1NF — each column stores only one value per row
- 2NF — every column depends on the full primary key
- 3NF — every column depends only on the primary key

ACID properties guarantee reliability:
- Atomicity — all or nothing
- Consistency — always valid
- Isolation — no interference
- Durability — permanently saved

Most important lesson:
A strong foundation makes everything built on 
top of it more reliable. Design well from the start.
