# Integrity Rules in Databases

Each user's or record should have a unique identifier as two taxpayers or customers with the same government or customer identifier would violate the entity integrity rule, as it leads to duplicate records and makes it impossible to uniquely identify individuals.

A shipment associated with the wrong order would violate the referential integrity rule because it creates an invalid relationship between the shipment and the order. It indicates that the shipment is linked to an order that doesn't exist or isn't the intended one.

## Primary and Foreign keys

A primary key is a column or set of columns that uniquely identifies each row in a table. It cannot contain null values and must have unique values for each row.

A foreign key is a column or set of columns in one table that refers to the primary key of another table. It establishes a link between the two tables based on the relationship between the referenced columns.

Entity integrity ensures that each row in a table can be uniquely identified. It requires that every table has a primary key, and that the primary key column(s) cannot contain null values.

Referential integrity ensures that relationships between tables are valid. It requires that foreign key values in one table must match primary key values in the related table or be null if allowed.

## Null values

A null value indicates a missing or unknown value in a column. It signifies that the actual value is not available or not applicable for that particular row.

## Database Diagrams

A database diagram visually represents the structure of a database, including tables, columns, primary keys, foreign keys, and relationships between tables. It's essential for understanding the database schema and formulating queries that combine data from multiple tables.

In a database diagram, a solid line connecting two tables represents a relationship where the foreign key in the child table cannot have null values. It indicates a mandatory relationship.A dashed line connecting two tables in a database diagram represents a relationship where the foreign key in the child table can have null values. It indicates an optional relationship.
