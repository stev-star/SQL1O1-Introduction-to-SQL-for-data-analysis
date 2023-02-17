# SQL1O1:Introduction-to-SQL-for-data-analysis

SQL  for Data Analysis

SQL is the "meat and potatoes" of data analysis. It's used for accessing, cleaning, and analyzing data that's stored in databases. It's very easy to learn, yet it's employed by the world's largest companies to solve incredibly challenging problems. 

## What is SQL?

SQL which stands for Structured Query Language is the standard computer language used for a database system — or rather a relational database management system. 
SQL is one of the most commonly used and flexible languages, as it combines a surprisingly accessible learning curve with a complex depth that lets users create advanced tools and dashboards for data analytics.


## Why  do data analyst need SQL? 
- SQL skills are in high demand.  The pure amount of data produced globally continues to grow at an alarming rate With this increase in the quantity of data has also    come substantial growth in the application of that data across industries. From data science to marketing, to healthcare, professionals with the SQL skills            necessary to properly handle this large amount of data are in increasingly high demand.

- SQL is easy to use. it’s simple and easy to learn compared to some of the more complex processes  For example, languages like Java require memorization of a series    of steps to complete a task, whereas SQL uses declarative statements to pull data.

- SQL has a variety of proprietary tools with their own specific focus, such as Microsoft SQL Server, PostgreSQL, and MySQL, that allow users to quickly create and       interact with databases.

- Vast amounts of data can be accessed directly where it is stored so that Data Analysts don’t have to copy data into other apps.
    
    
## Data Definition Language(DDL) 

Data Definition Language commands in SQL are used for changing the structure of a table. In other words, they are capable of creating, deleting, and modifying data.All commands are auto-committed which means that changes made by them are automatically saved in the database. 

#### CREATE
Used to create tables or databases.
``` SQL
CREATE TABLE <table name> ( 
        <attribute name 1> <data type 1>,
        ...
        <attribute name n> <data type n>);
```
#### ALTER
Used to modify the values in the table. We can also ALTER the datatype of the column and drop the columns by using the Alter Statement.
```SQL
ALTER TABLE <table name>
        ADD CONSTRAINT <constraint name> PRIMARY KEY (<attribute list>);
```
#### DROP
Deletes the table from the database.
```SQL
DROP TABLE <table name>;
```

```SQL
ALTER TABLE <table name>
DROP CONSTRAINT <constraint name>;
```
#### RENAME
Used to rename the table or database name.

#### TRUNCATE 
It removes all the rows from the table. It cannot be used with the Where condition. It never rollbacks.

## Data Query Language(DQL) 

DQL stands for Data Query Language. DQL command is used to retrieve data from the database.
SELECT:Used to fetch the data from a database or table.


## Data Manipulation Language(DML) 
stands for Data Manipulation Language. DML commands are used to store, modify, and delete data in the database. 
#### INSERT
Used to insert the new rows in the table.
```SQL
INSERT INTO <table name>
        VALUES (<value 1>, ... <value n>);
```
#### UPDATE
Used to update the values in the existing rows in the table.
```SQL
UPDATE <table name>
        SET <attribute> = <expression>
        WHERE <condition>;
```
#### DELETE
Used to delete a row or entire table. It can be used with the Where condition. It can be rolled back.
```SQL
DELETE FROM <table name>
        WHERE <condition>;
```
#### MERGE
Used to join two rows in the existing tables.



## Data Control Language(DCL)

DCL stands for Data Control Language. DCL commands are used for specifying permissions, access control and providing security to database objects. Examples of DCL statements are:
#### GRANT
Used to provide access to the user.
#### REVOKE
Used to take back the access privileges from the users.



## TCL Transaction Control Language (TCL)

TCL stands for Transaction Control Language. A transaction is a set of one ore more SQL commands that change data in the Oracle database. TCL commands are used for managing changes affecting the data in the database. Examples of TCL statements are:

#### COMMIT
Commits a Transaction.
#### SAVEPOINT
Sets a save point within a transaction which can be rollback as needed.
#### ROLLBACK
Rollbacks a transaction in case of any error occurs to certain SAVEPOINT
