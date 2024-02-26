- [**Basics**](#basics)
  - [What is SQL](#what-is-sql)
    - [Domain specific programming language](#domain-specific-programming-language)
  - [What SQL can do ?](#what-sql-can-do-)
    - [Using SQL in your websites](#using-sql-in-your-websites)
  - [DBMS](#dbms)
  - [RDBMS](#rdbms)
- [SQL Syntax](#sql-syntax)
  - [SQL statements](#sql-statements)

# **Basics**
## <h3>What is SQL</h3>
  - SQL stands for Structured Query Language.
  - SQL is a domain specific programming language, it can work with domain called as Database.
  - It's programming language designed for managing and manipulating relational database.
  - its provides a standardized way to communicate with database.

### Domain specific programming language 
   - The language which is used to build only a single part or domain of an application is called Domain specific programming language 
   - its capable of working with only single part or domain of an applications. 
   - **Example** :SQL, No SQL.
<p align="right">(<a href="#top">˄</a>)</p>

## What SQL can do ?
  - SQL can execute queries against a database 
  - SQL can retrieve data from a database
  - SQL can insert records in a database
  - SQL can update records in a database
  - SQL can delete records from a database
  - SQL can create new databases
  - SQL can create new tables in a database
  - SQL can create stored procedures in a database
  - SQL can create views in a database
  - SQL can set permissions on tables, procedures, and views

### Using SQL in your websites 
  - To build a web site that shows data from a database, you will need:

    * An RDBMS database program (i.e. MS Access, SQL Server, MySQL)
    * To use a server-side scripting language, like PHP or ASP
    * To use SQL to get the data you want
    * To use HTML / CSS to style the page
  
  <p align="right">(<a href="#top">˄</a>)</p>
  
## <h3>DBMS</h3>
   -  A database management system (DBMS) is system software for creating and managing databases.
   
   -  A Database Management System (DBMS) is a software system that is designed to manage and organize data in a structured manner. It allows users to create, modify, and query a database, as well as manage the security and access controls for that database.

<p align="right">(<a href="#top">˄</a>)</p>

## <h3>RDBMS</h3>
  - RDBMS stands for Relational Database Management System.

  - RDBMS is the basis for SQL, and for all modern database systems such as MS SQL Server, IBM DB2, Oracle, MySQL, and Microsoft Access.

  - The data in RDBMS is stored in database objects called tables. A table is a collection of related data entries and it consists of columns and rows.

     * Look at the "Customers" table :  
  -  **Example**  
```SQL
   SELECT * FROM Customers;
```   
<p align="right">(<a href="#top">˄</a>)</p>

# <h3>SQL Syntax</h3>
## <h4>SQL statements</h4>
  - SQL statements consists of keywords that are easy to understand. 
  - **Example**
  
      * select all records from customers tables :
```sql
   SELECT * FROM Customers;
```   