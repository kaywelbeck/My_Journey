
## 1. What is the difference between a relational and a non-relational database? 🗄️

- **Relational Database**: Stores data in rows and columns using structured tables. Schemas are used to organise data, while foreign keys are used to maintain relationships between tables (e.g., MySQL, PostgreSQL).                 
- **Non-Relational Database**: Stores data in a more flexible format, such as key-value pairs, documents, graphs, or wide-column stores. It does not require a fixed schema and is designed to scale out easily (e.g., MongoDB, Cassandra).

---

## 2. What are indexes? 📊

- **Indexes**: Special data structures that improve the speed of data retrieval operations on a database table at the cost of additional storage space. Indexes allow the database to find and access rows more quickly without scanning the entire table.

---

## 3. What are primary keys and secondary keys? 🔑

- **Primary Key**: A unique identifier for each record in a table, ensuring that no two rows can have the same primary key value. It cannot contain NULL values.
- **Secondary Key**: An additional key that is used to access data. Unlike primary keys, secondary keys can contain duplicate values and can be used for searching or sorting.

---

## 4. What are inner joins and outer joins? 🔗

- **Inner Join**: Combines rows from two or more tables based on a related column, returning only the rows that have matching values in both tables.
- **Outer Join**: Returns all the rows from one table and the matched rows from the second table. If there is no match, NULL values are returned for columns of the non-matching table. Types include:
  - **Left Outer Join**: Returns all rows from the left table and matched rows from the right.
  - **Right Outer Join**: Returns all rows from the right table and matched rows from the left.
  - **Full Outer Join**: Returns all rows when there is a match in either table.

---

## 5. What is the difference between DROP TABLE and TRUNCATE TABLE? 🗑️

- **DROP TABLE**: Completely removes a table from the database, including its structure and all the data stored in it. This action cannot be undone.
- **TRUNCATE TABLE**: Removes all rows from a table but keeps the table structure intact. This action is faster than DELETE because it does not log individual row deletions and can reset identity columns.

---

## 6. What are the different data types in SQL? 📅

Common SQL data types include:

- **Integer Types**: INT, BIGINT, SMALLINT
- **Decimal Types**: DECIMAL, FLOAT, REAL
- **String Types**: CHAR, VARCHAR, TEXT
- **Date and Time Types**: DATE, TIME, DATETIME, TIMESTAMP
- **Binary Types**: BLOB, BINARY

---

## 7. What are the WHERE and HAVING clauses used for? 📋

- **WHERE Clause**: Filters records before any groupings are made. It is used to specify the conditions for selecting rows from a table.
- **HAVING Clause**: Filters records after the GROUP BY operation has been applied. It is used to specify conditions on aggregate functions.
