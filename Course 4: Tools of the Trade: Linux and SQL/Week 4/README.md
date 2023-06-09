# Week 4
# Databases and SQL

# Introduction to SQL and Databases

A database is an organized collection of information or data that can store massive amounts of data and be accessed by multiple people simultaneously. Databases can perform complex tasks while accessing data. Relational databases, which we'll focus on in this course, consist of tables that are related to each other. Each table contains columns (fields) and rows (records). The columns represent the fields of information, while the rows contain specific data related to the columns. Multiple tables in a relational database can be connected through common columns, known as keys. The primary key is a unique identifier for each row, while the foreign key connects tables together. A table can have only one primary key, but multiple foreign keys.


As a security analyst, it's crucial to be familiar with databases and the tools used to access them. SQL (Structured Query Language) is an essential tool for working with databases. SQL is a programming language used to create, interact with, and request information from a database. It allows analysts to retrieve logs and search for specific data points efficiently. For example, SQL can help identify improperly configured machines or detect unusual patterns indicating potential malicious activity. SQL is also valuable for basic data analytics, enabling analysts to filter data and make informed security-related decisions, such as identifying machines that need patch updates or determining optimal update times.

# SQL Queries

To determine which computer is assigned to a specific employee, we can use SQL queries. Given the employees table with columns like employee_id and device_id, we write a query using the SELECT and FROM keywords. SELECT specifies the columns to return, and FROM indicates the table to query. By running this query, we obtain the desired information on employees and their assigned computers. SQL syntax rules state that keywords are not case-sensitive, and semicolons mark the end of a statement. To retrieve additional information, such as department, username, or office, we can use the asterisk (*) to select all columns from the table, resulting in the complete table output.

Filtering is a powerful feature of SQL that allows us to select specific data from a database based on certain conditions. It is akin to choosing only the data we want, similar to selecting fresh apples from a fruit cart. As a security analyst, filtering can help us narrow down information in logs, such as selecting login attempts from a specific country. SQL utilizes operators, such as the equal to operator (=), to define conditions for filtering. The WHERE clause is used to specify the filter condition in SQL queries. By adding the WHERE clause to our SELECT and FROM statements, we can apply filters to retrieve desired data. We can create simple filters that match exact values or more complex filters that search for patterns using wildcard characters like the percentage sign (%). For pattern matching, the LIKE operator is used instead of the equal to operator, allowing us to search for specific patterns in a column. By combining operators, keywords, and the WHERE clause, we can construct SQL queries to filter data effectively. This capability empowers security analysts to extract relevant information from databases and perform more targeted analysis.

# More SQL Filters

In databases, there are three common data types: string, numeric, and date and time. String data consists of ordered sequences of characters, such as user names. Numeric data consists of numbers and allows mathematical operations. Date and time data represents specific dates and/or times.
As a security analyst, you will often work with numeric and date and time data types when querying databases. Operators play a crucial role in filtering these data types. Common operators for numeric and date and time data include equals, greater than, less than, not equal to, greater than or equal to, and less than or equal to. For example, you can filter log-in attempts made after 6 pm using the greater than operator. By constructing SQL queries with the SELECT, FROM, and WHERE clauses, you can apply these filters to retrieve relevant data.
Another useful operator for filtering is BETWEEN, which allows you to specify a range of values. For instance, you can find all the patches installed between two specific dates by using the BETWEEN operator in your query. By indicating the column to filter, the BETWEEN operator, the starting point of the range, the keyword AND, and the end point of the range, you can retrieve the desired data.
By understanding these operators and utilizing them in SQL queries, security analysts can effectively filter and retrieve numeric and date and time data from databases, enabling them to perform targeted analysis and identify patterns or anomalies in the data.


In SQL, when dealing with complex security analysis tasks, it is often necessary to filter queries based on multiple conditions. To accomplish this, the AND operator is used to specify that both conditions must be met simultaneously. For example, when selecting machines that use a specific email client and operating system, the query should return only those machines that satisfy both conditions. This is similar to selecting large and fresh apples from a box, excluding small apples and rotten ones. By using the AND operator in SQL, the query can filter the data accordingly.

To implement the AND operator in SQL, the query begins with the SELECT statement, followed by specifying the conditions in the WHERE clause. Each condition is separated by the AND operator. By combining the conditions using AND, the query will retrieve results that meet all specified criteria.

On the other hand, the OR operator allows for the selection of rows that satisfy either one of the conditions, or even both. In SQL, the OR operator is used to join conditions, indicating that either condition can be met. This operator is useful when, for example, selecting machines that require a patch for either OS 1 or OS 3.

Additionally, the NOT operator can be used to negate a condition. It is employed to select entries that do not match a specific condition. This can be helpful when, for instance, updating all devices except those running a particular operating system.

By using these operators effectively in SQL queries, security analysts can filter data based on multiple conditions, allowing them to perform complex analysis and efficiently retrieve the desired information.

# SQL Joins


Joining tables in SQL allows us to combine information from multiple tables in a database. This is particularly useful when we need to retrieve data that is spread across different tables. For example, by joining a table that lists security vulnerabilities with another table that contains information about machines in a company, we can generate a list of vulnerable machines.

To perform a join in SQL, we need to specify the syntax correctly. When working with two tables, it's essential to indicate which table we're selecting columns from to avoid ambiguity. This is done by writing the table name followed by a period and then the column name. This syntax helps SQL understand the specific column we're referring to.

To join tables, we first identify a shared column that acts as a connection point between the two tables. This shared column is typically a primary key in one table and a foreign key in the other. By using this shared column, we can establish relationships between the tables.

The INNER JOIN is a type of join that returns rows where the specified column matches in both tables. By selecting the primary key column from both tables, we can identify matching rows and retrieve all columns from both tables for those matches.

It's important to consider NULL values when joining tables. In SQL, NULL represents missing or unknown values. For example, in the case of unassigned machines, the employee_id column may have NULL values. These NULL values need to be considered when performing joins.

To execute a join in SQL, we construct the query by specifying the tables to join, the join type (e.g., INNER JOIN), and the column to base the join on. The common column is identified by including the table name followed by a period and then the column name for both tables.

By combining the tables through a join, we can retrieve the desired information, selecting specific columns from both tables. The query results will display the records that match on the specified column, including columns from both tables.

By mastering the concept of joining tables in SQL, security analysts can efficiently gather information from different tables and gain valuable insights for their analysis tasks.


In addition to inner joins, outer joins provide a way to retrieve all entries from one or both tables, even without matching columns. There are three types of outer joins: LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN.

A LEFT JOIN returns all records from the first table and only the matching rows from the second table based on a specified column. The non-matching rows from the first table are included with NULL values for the columns from the second table.

A RIGHT JOIN returns all records from the second table and only the matching rows from the first table based on a specified column. The non-matching rows from the second table have NULL values for the columns from the first table.

A FULL OUTER JOIN returns all records from both tables, including all columns. NULL values are assigned to the columns that do not have a matching value in either table.

To implement these joins in SQL, the syntax structure is similar to INNER JOIN, but with keywords like LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN.

As a security analyst, it's not necessary to memorize all the details of these joins. Once you understand the type of join needed, you can easily search for the specific syntax and information required to execute the queries.

Understanding joins, including outer joins, is crucial knowledge for security analysts using SQL to efficiently retrieve and analyze data from multiple tables.

# Glossary terms from week 4
Terms and definitions from Course 4, Week 4
Database: An organized collection of information or data

Date and time data: Data representing a date and/or time

Exclusive operator: An operator that does not include the value of comparison

Filtering: Selecting data that match a certain condition

Foreign key: A column in a table that is a primary key in another table 

Inclusive operator: An operator that includes the value of comparison

Log: A record of events that occur within an organization's systems

Numeric data: Data consisting of numbers

Operator: A symbol or keyword that represents an operation

Primary key: A column where every row has a unique entry

Query: A request for data from a database table or a combination of tables

Relational database: A structured database containing tables that are related to each other

String data: Data consisting of an ordered sequence of characters

SQL (Structured Query Language): A programming language used to create, interact with, and request information from a database

Syntax: The rules that determine what is correctly structured in a computing language

Wildcard: A special character that can be substituted with any other character
