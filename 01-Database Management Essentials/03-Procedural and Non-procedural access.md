# Procedural and Non-procedural Access

Procedural access and non-procedural access are two different ways of interacting with a database, particularly in how data is retrieved.

Procedural access requires a user to write detailed computer programs that specify how to navigate through the database to access the data. This involves writing code with loops and other complex procedural logic. In early DBMSs, there was a close connection between a database and computer programs that accessed the database. Essentially, the DBMS was considered part of a programming language.

Second-generation database systems were "navigational," meaning programmers had to write code to navigate among a network of linked records.

- Procedural access involves coding complex procedures with loops.
- Procedural languages have statements like "for" and "while" for looping.

Non-procedural access allows users to specify what data to retrieve, rather than how to retrieve it. Users do not need to write complex procedures with loops.

- Non-procedural languages do not have looping statements.
- Non-procedural access reduces the amount of code needed by a factor of 100 compared to procedural access.

The standard tool for non-procedural access is the SQL SELECT statement. Most DBMSs provide an SQL client to enter and execute SQL statements. Many DBMSs also offer graphical tools to access databases, where users indicate the required tables, relationships, and columns, and the system generates the plan to retrieve the data.

Non-procedural access, particularly through SQL, has revolutionized how users interact with databases, making it more accessible, efficient, and productive than procedural access. While procedural languages remain important for complex applications, non-procedural access is a cornerstone of modern database management.
