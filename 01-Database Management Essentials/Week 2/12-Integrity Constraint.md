# Integrity Constraint

Constraint names are crucial for identifying and troubleshooting errors related to data integrity violations. Meaningful names provide context and clarity when a constraint is violated, aiding in faster resolution.

A meaningful constraint name helps a database administrator (DBA) quickly understand the nature of the error when a constraint violation occurs. A generic or meaningless name offers little help in diagnosing the problem.",

## Constraint types

- Primary Key:Ensures each row has a unique identifier and prevents null values in the primary key column(s).
- Foreign Key: Establishes relationships between tables by ensuring that values in the foreign key column(s) match values in the primary key column(s) of the related table
- Unique: Ensures that all values in a column or a set of columns are unique, preventing duplicate entries (other than nulls, which can be duplicated). Not used for primary keys, as uniqueness is already implied.
- Required (NOT NULL): Specifies that a column cannot have a null value. A value must always be provided.
- Check:Defines a condition that must be met for any value inserted into the column. Used to restrict the range of valid values.

Constraints can be defined inline as part of a column definition or externally after all column definitions. Constraints involving multiple columns must be defined externally.While constraint names are often optional, it's considered best practice to always name constraints using descriptive names. This aids in debugging and maintenance.

```SQL

--Unique
CREATE TABLE courses (
    course_id INT PRIMARY KEY,
    course_name VARCHAR(100) UNIQUE,
    duration INT
);

--Not Null
CREATE TABLE teachers (
    teacher_id INT PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    subject VARCHAR(50)
);

--Foreign key
CREATE TABLE departments (
    department_id INT PRIMARY KEY,
    department_name VARCHAR(100)
);

CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    name VARCHAR(50),
    department_id INT,
    FOREIGN KEY (department_id) REFERENCES departments(department_id)
);

--Check
CREATE TABLE orders (
    order_id INT PRIMARY KEY,
    order_date DATE,
    quantity INT CHECK (quantity > 0)
);

--Default
CREATE TABLE products (
    product_id INT PRIMARY KEY,
    product_name VARCHAR(100),
    price DECIMAL(10, 2) DEFAULT 0.00
);

--Index
CREATE TABLE customers (
    customer_id INT PRIMARY KEY,
    name VARCHAR(50),
    email VARCHAR(100)
);

CREATE INDEX idx_email ON customers(email);

--Primary key
CREATE TABLE enrollments (
    student_id INT,
    course_id INT,
    enrollment_date DATE,
    PRIMARY KEY (student_id, course_id)
);

```
