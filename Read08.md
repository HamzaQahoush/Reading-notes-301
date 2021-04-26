### What is SQL?

SQL (pronounced "ess-que-el") stands for Structured Query Language. SQL is used to communicate with a database. it is the standard language for relational database management systems.

SQL statements are used to perform tasks such as update data on a database, or retrieve data from a database
The standard SQL commands such as "Select", "Insert", "Update", "Delete", "Create", and "Drop" can be used to accomplish almost everything that one needs to do with a database.


### Table Basics

A relational database system contains one or more objects called tables. The data or information for the database are stored in these tables. 
Tables are uniquely identified by their names and are comprised of columns and rows. Columns contain the column name, data type, and any other attributes for the column. Rows contain the records or data for the columns


### Selecting Data
The select statement is used to query the database and retrieve selected data that match the criteria that you specify. Here is the format of a simple select statement:
select "column1"

  `[,"column2",etc] 
  from "tablename"
  [where "condition"];
  [] = optional`

If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (*)


The where clause (optional) specifies which data values or rows will be returned or displayed, based on the criteria described after the keyword where.
Conditional selections used in the where clause:

`=	Equal`
`>	Greater than`
`<	Less than`
`>=	Greater than or equal`
`<=	Less than or equal`
`<>	Not equal to`

