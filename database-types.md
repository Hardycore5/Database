## Database Types

Not all databases work the same way. Different types of 
databases exist because different problems need 
different solutions.

This file explains the main types of databases, 
what makes each one special, and when to use each one.

Choosing the right type of database for your project 
is one of the most important decisions a developer makes.

## Relational Databases
A relational database stores information in tables that are 
connected to each other through relationships.

It is the most widely used type of database in the world.

Examples:
- MySQL — used by Facebook, Twitter, and YouTube
- PostgreSQL — used by Instagram and Spotify
- SQLite — lightweight database used in mobile apps

Best used when:
Your information is structured, organized, and the 
relationships between data are important.

## NoSQL Databases
A NoSQL database stores information in a flexible way 
that does not always use tables.

NoSQL stands for "Not Only SQL" — meaning it can store 
information in many different formats.

Examples:
- MongoDB — stores data as flexible documents
- Firebase — used in many mobile apps
- Redis — stores data as simple key-value pairs

Best used when:
Your information changes frequently, is unstructured, 
or needs to be stored and retrieved very quickly.

## SQL vs NoSQL — When to Use Each

| Feature | SQL | NoSQL |
|---|---|---|
| Structure | Fixed tables and columns | Flexible, varies by type |
| Best for | Structured, organized data | Unstructured, changing data |
| Examples | MySQL, PostgreSQL | MongoDB, Firebase |
| Relationships | Strong relationships between tables | Limited relationships |
| Scalability | Scales vertically | Scales horizontally |

Simple rule:
- Use SQL when your data is structured and organized.
- Use NoSQL when your data is flexible or changes often.

## Document Databases
A document database is a type of NoSQL database that 
stores information as documents — similar to JSON files.

Each document can have a different structure, making it 
very flexible for storing complex or changing data.

Example of a document:
{
  "name": "Emeka",
  "age": 10,
  "class": "Grade 5",
  "subjects": ["Maths", "English", "Science"]
}

Popular document databases:
- MongoDB
- CouchDB

Best used when: Your data has varying fields and structures.
