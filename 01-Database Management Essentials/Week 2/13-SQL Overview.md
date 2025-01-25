# SQL Overview

SQL is sometimes pronounced `\sequel\` due to its historical evolution from the `\SEQUEL\` language developed by IBM.

SQL standards compliance is weaker compared to web standards like HTML5. There's no mandatory conformance testing for SQL, relying on vendor self-reporting, leading to variations in implementations. Web standards have robust conformance testing and validation processes (e.g., W3C validation, Acid3 tests) ensuring greater consistency across browsers.

Conformance to the SQL standard varies significantly among database vendors. While core features often have good support, optional features and extensions show greater divergence. This lack of strict adherence hinders portability of SQL code between different database systems.

The weak SQL conformance stems from a trade-off between portability and vendor control/innovation. Vendors prioritize introducing proprietary features and extensions to differentiate their products, potentially sacrificing cross-platform compatibility.

Weak conformance to SQL standards leads to the following:

- Reduced portability.
- Higher switching costs.
- Vendor lock-in.

SQL evolved from IBM's SQUARE language, later renamed SEQUEL and then SQL due to legal reasons. It has become the dominant language for managing relational databases.

## SQL Contexts

- Standalone: Users directly interact with the database using an SQL editor (like SQL Developer) to execute SQL statements.
- Embedded: SQL statements are integrated within a host programming language (like Java or Visual Basic) and executed by the program."

## Parts of SQL

- Data Definition Language (DDL): Used to define database objects (e.g., CREATE TABLE).- Data Manipulation Language (DML): Used to retrieve and modify data (e.g., SELECT, INSERT, UPDATE, DELETE).
- Data Control Language (DCL): Used to manage access and permissions (e.g., GRANT, REVOKE).
