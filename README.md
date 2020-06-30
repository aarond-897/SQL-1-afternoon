# SQL-1-afternoon

--TABLE-PERSON

-- 1.
-- CREATE TABLE person(
-- id SERIAL PRIMARY KEY,
-- name VARCHAR(30),
-- age INT,
-- height INT,
-- city VARCHAR(30),
-- favorite_color VARCHAR(30)
-- );

-- 2.
-- INSERT INTO person
-- (name, age, height, city, favorite_color)
-- VALUES
-- ('Rich', 27, 180, 'Phoenix', 'orange');

-- 3.
-- SELECT \* FROM person
-- ORDER BY height DESC;

-- 4.
-- SELECT \* FROM person
-- ORDER BY height ASC;

-- 5.
-- SELECT \* FROM person
-- ORDER BY age DESC;

-- 6.
-- SELECT \* FROM person
-- WHERE age > 20;

--7.
-- SELECT \* FROM person
-- WHERE age = 18;

--8.
-- SELECT \* FROM person
-- WHERE age < 20 OR age >30;

--9.
-- SELECT \* FROM person
-- WHERE age !=27;

--10.
-- SELECT \* FROM person
-- WHERE favorite_color != 'red';

-- 11.
-- SELECT \* FROM person
-- WHERE favorite_color NOT IN ('red','blue');

-- 12.
-- SELECT \* FROM person
-- WHERE favorite_color IN('orange', 'green');

--13.
-- SELECT \* FROM person
-- WHERE favorite_color IN('orange', 'green', 'blue');

-- 14.
-- SELECT \* FROM person
-- WHERE favorite_color IN('yellow', 'purple');

--Table-orders
-- 1.
-- CREATE TABLE orders(
-- order_id SERIAL PRIMARY KEY,
-- person_id INT,
-- product_name VARCHAR(30),
-- product_price FLOAT,
-- quantity INT
-- );

-- 2.
-- INSERT INTO orders
-- (product_price, person_id, quantity, product_name)
-- VALUES
-- (1.00,3, 7, 'Casette');

--3.
-- SELECT \* FROM orders;

--4.
-- SELECT SUM(quantity) FROM orders;

--5.
-- SELECT SUM(product_price \* quantity) FROM orders;

--6.
-- SELECT SUM(product_price \* quantity) FROM orders
-- WHERE person_id =2;

-- TABLE-ARTIST

-- 1.
-- INSERT INTO artist
-- (name)
-- values
-- ('Saint Pepsi');

-- 2.
-- SELECT \* FROM artist
-- ORDER BY name DESC LIMIT 10;

--3.
-- SELECT \* FROM artist
-- ORDER BY name ASC LIMIT 5;

--4.
-- SELECT \* FROM artist
-- WHERE name LIKE 'Black%';

--5.
-- SELECT \* FROM artist
-- WHERE name LIKE '%Black%';

--Table-Employee

-- 1.
-- SELECT first_name, last_name FROM employee
-- WHERE city = 'Calgary';

--2.
-- SELECT birth_date FROM employee
-- ORDER BY birth_date DESC LIMIT 1;

-- 3.
-- SELECT birth_date FROM employee
-- ORDER BY birth_date ASC LIMIT 1;

--4.
-- SELECT first_name, last_name, employee_id FROM employee
-- WHERE first_name='Nancy' AND last_name='Edwards';

-- SELECT \* FROM employee
-- WHERE reports_to=2;

--5.
-- SELECT COUNT(\*) FROM employee
-- WHERE city='Lethbridge';

-- Table-invoice
-- 1.
-- SELECT COUNT(\*) FROM invoice
-- WHERE billing_country ='USA';

-- 2.
-- SELECT MAX(total) FROM invoice;

--3.
-- SELECT MIN(total) FROM invoice;

--4.
-- SELECT \* FROM invoice
-- WHERE total > 5;

-- 5.
-- SELECT COUNT(\*) FROM invoice
-- WHERE total <5;

--6.
-- SELECT COUNT(\*) FROM invoice
-- WHERE billing_state IN ('CA','TX','AZ');

--7.
-- Select AVG(total) FROM invoice;

--8.
-- SELECT SUM(total) FROM invoice;
