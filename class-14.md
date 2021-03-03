# Class 14

* ##  Database Normalization
Normalization is a technique for organizing data in a database. It is important that a database is normalized to minimize redundancy (duplicate data) and to ensure only related data is stored in each table. It also prevents any issues stemming from database modifications such as insertions, deletions, and updates.
---
First Normal Form (1NF):

Data is stored in tables with rows uniquely identified by a primary key
Data within each table is stored in individual columns in its most reduced form
There are no repeating groups

Second Normal Form (2NF):

Everything from 1NF
Only data that relates to a table’s primary key is stored in each table

Third Normal Form (3NF):

Everything from 2NF
There are no in-table dependencies between the columns in each table

Note that there are actually six levels of normalization; however, the third normal form is considered the highest level necessary for most applications so we will only be discussing the first three forms.

The database we will be working with in this tutorial is for Codey’s Construction company `(Codey is a helpful coding bot that works with you in the course mentioned earlier)`. As you can see from the schema above, the database contains the tables projects, job_orders, employees, and project_employees. Recently, the customers table was added to store customer data.

Unfortunately, this table has not designed in a way that satisfies the three forms of normalization… Let’s fix that!