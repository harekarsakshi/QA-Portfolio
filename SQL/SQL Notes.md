# SQL Notes

## Database
A database is a collection of organized data.

## Table
A table stores data in rows and columns.

## Row
A single record in a table.

## Column
An attribute or field in a table.

## Primary Key
A unique identifier for each row.

## First SQL Queries

### Show all data

SELECT * FROM users;

### Show only names

SELECT name FROM users;

### Find user with ID 1

SELECT * FROM users
WHERE id = 1;

SELECT * FROM users
WHERE id = 2;

SELECT * FROM users
WHERE city = 'Orlando';

SELECT * FROM users
ORDER BY id;

SELECT * FROM users
ORDER BY id DESC;

SELECT * FROM users
WHERE city = 'Orlando'
AND id = 1;

SELECT * FROM users
WHERE city = 'Orlando'
OR city = 'Miami';

SELECT * FROM users
WHERE name LIKE 'S%';

SELECT * FROM users
WHERE name LIKE '%a';

SELECT * FROM users
WHERE city IN ('Orlando', 'Miami');

SELECT * FROM users
WHERE name LIKE 'A%';

SELECT * FROM users
WHERE name LIKE '%a';

SELECT * FROM users
WHERE name LIKE '%lex%';

SELECT * FROM users
WHERE id BETWEEN 1 AND 3;

SELECT users.name, orders.product
FROM users
INNER JOIN orders
ON users.user_id = orders.user_id;

SELECT students.name, courses.course
FROM students
LEFT JOIN courses
ON students.student_id = courses.student_id;

