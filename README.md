# SQL Assignment:

1) What is SQL? Why is it called a DSL?
ans) SQL (Structured Query Language) is a standard language used to store, retrieve, and manage data in relational       databases.
     It is known for its simplicity and powerful capabilities in handling structured data.
SQL is called a Domain-Specific Language (DSL) because it is designed specifically for database operations, unlike general-purpose languages like Python or Java.

2) Types of Languages: Declarative and Functional
ans) Declarative languages describe what the program should accomplish without specifying how to do it.  SQL is an        example—it tells the database what data is needed.
     Functional languages (like Haskell or Scala) are based on mathematical functions. They emphasize immutability, no side effects, and function composition to solve problems.

3) Difference Between Statement and Query
ans) A statement is a complete command that performs an action like creating tables or inserting data (e.g., CREATE, INSERT).
     A query is a request to retrieve data from the database, usually using SELECT.
Statements may or may not return results, but queries are meant to return data.

4) Difference Between Primary Key and Key
ans) A primary key is a specific type of key that uniquely identifies each record in a table and does not allow null values.
A key is a broader term used to refer to any attribute(s) that can be used to identify records (including primary, foreign, and candidate keys).
Every table can have only one primary key, but multiple keys can exist.

5) Difference Between DROP, TRUNCATE, and DELETE + Speed
ans) DROP permanently deletes the entire table structure and its data.
TRUNCATE removes all rows from a table but keeps its structure intact.
DELETE removes specific rows based on a condition and can be rolled back.
In terms of speed: DROP > TRUNCATE > DELETE (DROP is fastest, DELETE is slowest due to logging and conditions).

6) What are Isolation Levels?
ans) Isolation levels control how transactions interact with each other, especially when accessing or modifying data at the same time.
They ensure data consistency, integrity, and prevent issues like dirty reads, non-repeatable reads, or phantom reads.

Read Uncommitted:
This is the lowest isolation level. It allows one transaction to read data from another that hasn’t yet been committed.
This can lead to dirty reads, where data might be rolled back later, causing inconsistencies.

7) Define Normalization. What is 2NF and 3NF?
ans) Normalization is the process of organizing database tables to reduce redundancy and improve data integrity.
It involves breaking down large tables into smaller ones and defining relationships among them.

a) Second Normal Form (2NF):
A table is in 2NF if it is in 1NF and all non-key attributes are fully functionally dependent on the entire primary key (no partial dependencies).

b) Third Normal Form (3NF):
A table is in 3NF if it is in 2NF and all non-key attributes are only dependent on the primary key, not on other non-key columns (no transitive dependencies).