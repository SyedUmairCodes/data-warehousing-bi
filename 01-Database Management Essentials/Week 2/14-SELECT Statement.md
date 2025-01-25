# The SELECT Statement

Before formulating a query, understand the database structure including table names, column names, data types (numeric, text, date), and relationships between tables (especially for multi-table queries).

Use parentheses in logical expressions with AND and OR operators to explicitly define the order of evaluation and avoid ambiguity. This improves readability and ensures consistent behavior across database systems.

Query formulation is essential for application development and database management. Developers use queries to retrieve and manipulate data, while database specialists use them for data analysis and administration.

## Components of the SELECT Statement

- SELECT: Specifies the columns or expressions to be retrieved. '\*' retrieves all columns.
- FROM: Specifies the table(s) from which to retrieve data."
- WHERE: Filters rows based on specified conditions (optional)."
- ORDER BY: Sorts the result set based on specified column(s) (optional)."

An expression is a combination of columns, operators, functions, and constants that produces a value. It can be used wherever a column can be used (e.g., in SELECT, WHERE clauses).

> Use compatible data types in comparisons. Compare numeric columns with numeric constants, text columns with text constants, and date columns with date constants.

Text comparisons (e.g., in WHERE clauses) are often case-sensitive. Ensure consistent casing in comparisons. Use the DISTINCT keyword in the SELECT clause to eliminate duplicate rows in the result set.

Functions for manipulating dates (e.g., extracting the year) can vary between database systems (e.g., Oracle and PostgreSQL).
