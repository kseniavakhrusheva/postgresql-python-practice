# PostgreSQL and Python Database Practice

## Project Description

This repository contains university laboratory work focused on designing and managing relational databases in PostgreSQL using Python.

The project demonstrates implementation of database operations through separate Python functions and safe interaction with the database using parameterized SQL queries.

---

## Initial Task
 Crop Production

The database stores information about:

- districts;
- regions;
- administrative heads;
- crops;
- crop families;
- crop yields for the last three years.

Database schema includes:

- Districts
- Crops
- CropYields

---

## Implemented Functionality

### Database Structure

- database creation in PostgreSQL;
- table creation using CREATE statements;
- primary and foreign key implementation;
- maintaining data integrity.

### Insert Operations

- insert a single record;
- insert multiple records;
- parameterized INSERT queries.

### Select Operations

- select all records;
- select records using conditions;
- perform JOIN operations;
- parameterized filtering.

### Update Operations

- update table fields;
- preserve referential integrity.

### Delete Operations

- delete records using conditions;
- delete all records.

### Security

All SQL queries were implemented using parameterized queries through psycopg2 to avoid SQL injection.

Example:

```python
cur.execute(
    "SELECT * FROM users WHERE username = %s",
    (username,)
)
```

---

## Technologies

- Python
- PostgreSQL
- SQL
- psycopg2
- Jupyter Notebook

---

## Project Structure

```

postgresql-python-practice/
│
├── README.md
├── postgresql_python_lab.ipynb

```

---

## Learning Outcomes

During this laboratory work the following skills were developed:

- relational database design;
- SQL query writing;
- Python and PostgreSQL integration;
- CRUD operations;
- parameterized database interaction.
