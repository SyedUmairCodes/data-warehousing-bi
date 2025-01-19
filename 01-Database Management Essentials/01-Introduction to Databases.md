# Introduction to Databases

A database is a collection of persistent, interrelated, and shared data. Database Management Systems (DBMS) are collections of components that support the creation, use, and maintenance of databases.

- Data resides on stable storage like magnetic disks, which allows for repetitive use. Data is retained throughout its lifecycle but can be removed or archived when no longer relevant.
- Data stored in separate units are connected to provide a comprehensive picture. Databases store entities and the relationships between these entities.
- Databases are shared by many applications and users simultaneously.

## Data base Management Systems

A DBMS Includes tools for defining entity types, relationships, integrity constraints, and authorization rights. This is a feature that distinguishes DBMS from desktop software like word processors and spreadsheets. Planning is essential for databases, even small ones, and an Entity Relationship Diagram (ERD) should be developed before implementation.

- Allows users with limited computing skills to submit queries. Users specify what data to retrieve, not how to retrieve it. This is considered the most important feature because it allows access without detailed coding.
- Offers graphical tools to develop menus, data entry forms, and reports.
- Combines non-procedural access with the full capabilities of a programming language, such as Java or Javascript.
- Includes control mechanisms to prevent interference from simultaneous users and to recover lost data after a failure.
- Provides tools to monitor and improve database performance.
- DBMS have evolved to provide a wide range of features for these tasks.

### Types of DBMS

- Enterprise DBMSs designed to support large databases with many simultaneous users. They have strong reliability and performance requirements and typically run on powerful servers. Oracle is a leading provider of enterprise database products.
- Desktop DBMSs that support small workgroups with smaller databases and modest reliability. Microsoft Access dominates this market.
- Embedded DBMSs are sold as part of an application and are hidden from users.

### Evolution of DBMS

The evolution of database technology has resulted in four generations of products:

- First-generation: Supported sequential and random searching, requiring detailed computer programs to access data.
- Second-generation: True database management systems that managed multiple entity types and relationships. Still required computer programs to access data, also known as navigational systems because the programmer had to write code to navigate linked records.
- Third-generation: Relational DBMSs based on mathematical relations, with optimization technology to enable efficient access using non-procedural language. IBM was a pioneer in the development of this technology.
- Fourth-generation: Extended database technology to unconventional data such as images, videos, and web data, also known as object relational or object-oriented systems. They feature convenient ways to publish static and dynamic web data.

## Recent Innovations

- Cloud computing: Supports on-demand access to data and software, a new area of product development for established and new DBMS vendors.
- NoSQL: Developed to deal with the challenges of big data and stands for "not only SQL", which provides alternative technologies to SQL.
