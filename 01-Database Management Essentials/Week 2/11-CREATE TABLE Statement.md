# The CREATE TABLE Statement

The CREATE TABLE statement in SQL defines a new table within a relational database. It specifies the table's name, columns, data types for each column, and optional constraints to ensure data integrity.

SQL is a standardized language, enabling the CREATE TABLE statement to work across most database systems. However, database vendors often add proprietary extensions, limiting portability for advanced features. Precise syntax is crucial for CREATE TABLE. Even a minor error like a missing comma can prevent successful execution. Database systems have strict parsing rules.

```SQL

CREATE TABLE employees (
    employee_id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    phone_number VARCHAR(15),
    hire_date DATE NOT NULL,
    job_title VARCHAR(50) NOT NULL,
    department_id INT,
    salary DECIMAL(10, 2),
    manager_id INT,
    FOREIGN KEY (department_id) REFERENCES departments(department_id),
    FOREIGN KEY (manager_id) REFERENCES employees(employee_id)
);

```

## Data Types

- Char: Fixed-length character string; stores the maximum length specified, suitable for fixed-length data like state abbreviations
- VARCHAR: Variable-length character string; stores only the characters used, efficient for varying-length data like names. Oracle uses VARCHAR2."
- INTEGER: Whole numbers without decimal points"
- FLOAT: Floating-point numbers with specified precision for significant digits, used in scientific calculations or for values with varying decimal places"
- DECIMAL:Fixed-precision decimal numbers with a total of 'w' digits and 'r' digits after the decimal point, suitable for monetary values
- DATE: Stores date and time values. Some systems may have separate DATE, TIME, and TIMESTAMP types.

## GUI Interfaces

Due to the complexity and strict syntax of CREATE TABLE, many database systems provide visual tools to simplify table creation and modification.
