# SQL-Reference-Sheet

## How to Create a Database

- Create Database Statement
- can also use createdb program which uses create database statement behind the scenes
- primary key
- options are below:
- db_name: is the name of the new database to create
- name must be unique in the PostgreSQL database server
- if the name exists an error will be issues
- role_name: is the role name of the user who will own the new database
- PostgreSQL uses user's role name who executes the 'create database' statement
- template: template1 is the default template database
- encoding: specifies the character set
- encoding: utf=8
- owner: hr, assuming hr exists in the database server
- maximum concurrent connections: 25
- using queries can combine and filter data

### How to create a table

- syntax is
- CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  columnn3 datatype,
  ...
  );
- the column params specify the names of the columns
- datatype param specifies the type of data the column can hold (varchar, integer, date, etc.)
- three table views (content/ structure/ddl)
- insert data into table to create row (aka records)
- similiar to spreadsheets

#### How to get everything from a single table

- queries (select \* from database name)
- command is Execute Query
- use SELECT with .id

##### How to get one thing from a single table with a "where" clause

- execute all queries in the connection menu which executes all statements at once
- multiple matches of the same suggestions will be grouped by type,
- command clear results to clear the result area
- SELECT is the keyword used to query
- The SQL WHERE clause is used to specify a condition while fetching the data from a single table or by joining with multiple tables
- The WHERE clause is not only used in the SELECT statement, but it is also used in the UPDATE, DELETE statement, etc.
- SYNTAX: SELECT column1, column2, columnN 
FROM table_name
WHERE [condition]

###### how to add something to a table

- modify a record highlight cell and type change or select row
- copy paste

###### how to edit something inside a table

- highlight the row or data and type

###### how to remove something from a table

- Delete statement removes data from a table
- large table use truncate table statement - removes all rows from the table
- TRUNCATE TABLE table_name;


####### join statement

- a join statement is used in the where clause

- A JOIN clause is used to combine rows from two or more tables, based on a related column between them.
- (INNER) JOIN: returns records that have matching values in both tables
- LEFT (OUTER) JOIN: returns all records from the left table, and the matched records from the right table
- FULL (OUTER) JOIN: returns all records that match in either left or right table
