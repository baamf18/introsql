# introsql
My anotations while learning introduction to SQL and MySQL from the course Introduction to SQL by professor Chuck Russel

## First Part
* install of PHP and MYSQL servers with XAMPP
![image](https://user-images.githubusercontent.com/65134036/235553197-6bc22fdc-3af8-4a61-85a8-a34bcd5294b3.png)

* use of XAMPP to visualize a HTML page created in my machine through localhost connection

>  Questions:
- what is the best directory to put the xampp file and subdirectories?

## Second Part
* DataBases evolution and history
* Sequential Master Update
* National Institute of Standards and Technology
* DBs Servers: Oracle, MySQL -- Maria DB, HSQL, PostGRESQL, ...
* CRUD Operations

DATABASE // RELATION (TABLE) // TUPLES (ROWS) // ATTRIBUTES (COLUMNS/FIELDS)

### Basic SQL Operations
SHOW DATABASES;
CREATE DATABASE database_name DEFAULT CHARACTER SET ___;
USE database_name;

CREATE TABLE table_name (attributes DATATYPE, ...);

SELECT ____ FROM table_name;

INSERT INTO table_name (attributes) VALUE (data to insert);

UPDATE table_name SET new_data WHERE match_data;

DELE FROM table_name WHERE match_data;

ORDER BY; LIMIT; WHERE ___ LIKE '%char%';

### Data Types
* String Fields
* Text fields
* Binary Types
* Binary Large Objects (BLOB)
* Integer Numbers
* Floating Point Numbers
* Dates (timestamp: 1970 - 2037)

### Keys and Indexes
* AUTO_INCREMENT
* PRIMARY KEY: must be an integer (4 bytes), can not be the logical key (can change), neither a string (occupies a lot of space)
* FOREIGN KEY: another Relation's PRIMARY KEY which is used to reference the other Relation/Table's Tuple/Row
* Logical Key: used by the client, to searh for data, to read and analyze
* Hash and Trees Logic (as a way to reach data faster)
  - Hash: best for exact key matches
  - BTrees: best for prefix lookups or sorting

use of a convention

## Third Part
* Avoid vertical repetition of Data (especially if it's a String)
* Create logical Relation between Tables
* Correct understanding of Key Types and appropriate use

* Create Database and Tables (follow logical order of precedence to create tables) -> populate them // relate them through foreign keys
-> bring them together

JOIN ___ ON rules :: link tables

Bringing tables together through relations: the SELECT output is temporary, ephemeral. It doesn't use space in the database, and doesn't waste time or space!

## Fourth Part

* One-to-Many vs Many-to-Many relations
- Many-to-Many: use of a connector table // relationship table // junction table: these tables usually do not have a primary key! (Meta-primary key: combinantion of the foreign keys) 



