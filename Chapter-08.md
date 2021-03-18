# Database and Data Modelling

[toc]

## 8.01 Database 

### File based approach

- Record structure designed first
- Limitation is that record structure is fixed



### Relational Database approach

- DBMS software stores data and database definition in DB
- Program-Data Independence
  - The separating of the data-structure
  - Changes to data-structure are independent from programs accessing data
  - Attributes can be easily added and removed
- Concurrent access to data
  - Lock may be applied to DB preventing activity from all users
  - Less severe lock is table-level locking where tables are locked on a per table basis leaving other tables open
- DBMS contains a Query Generator and a Report Generator 
  - Time taken to create new query is minimal



### DBMS Software

- Provides
  - Backup
  - Security
  - Interrogation of data via SQL Queries
  - Controlled access to data with views
- Data Dictionary is a repository containing
  - DB Design
  - All objects used to create queries, views, & reports
- Data Integrity
  - DBMS uses data dictionary to perform validation check
  - Validation checks are set up a table design stage
- Data Security
  - Backup is a centralised task administered by the DBA
  - As all data is held centrally by the DBMS security is easier to implement than it would be in  a file based approach
- Backup and DB Management Tools
  - Garbage collection to improve performance
  - Option to change page-size or distribute DB amongst multiple files or disks
  - Enable backups to run concurrently
  - Create snapshots of the DB for archiving purposes
- Software Tools found in DBMS
  - Ability to create basic objects like tables and queries



## 8.02 Relational Database Modelling

### Relational Database Terminology

- Entity - item about which data is recorded
- Table - Implementation of data for an entity in a relational database software
- Tuple - Data for single row in table
- Attribute - A data item for an entity



- Table Notation 

  - > CUSTOMER (
    >
    > ​	**CustomerName**  <-- Primary Key
    >
    > ​	CustomerTown
    >
    > ​	CustomerAddress
    >
    > ​	ContactPerson
    >
    > )

- Primary Key
  - Every Tuple must be unique
  - If there is no suitable attribute then reference number attribute created. eg: **CustomerID**
  
- Candidate Key
  
  - Occurs when there are multiple attributes suitable to be Primary Key
  
- Secondary Key & Indexing
  
  - Any attribute that is index and not primary key is called the secondary key
  - Indexing makes data retrieval faster
  
- Relationships

  - 1 to 1 - Rare - Occurs between two tables created at different times
  - 1 to Many - Most Common
  - Many to Many

- Foreign Key

  - Primary Keys in each table are linked

- Referential Integrity

  - Data stored in tables must obey the relationships that exist



### Relational Design

- Entities have same name
- Relationship line shows degree of relationship
- Relationship can be labelled to to indicate its purpose



### Duplicated Data

### Normalisation Process

- First Normal Form - 1NF
  - States that there should be no repeated group of attributes
- Second Normal Form - 2NF
  - States that non-key attributes in table must be dependent on knowing all of the primary key
- Third Normal Form - 3NF
  - States that there must not be any dependency between any non-key attributes



## 8.03 Data Definition Language + Data Manipulation Language

### Data Definition Languages

- Industry standard for Data Definition Language and Data Manipulation Language is SQL

- DDL used for creation of database, DB Design, and the writing of queries

- DML used for create of queries and basic maintenance of records

- Creating a DB

  - > CREATE DATABASE TRAINING

- Creating a Table Definition

  - > CREATE TABLE STAFF
    >
    > (
    >
    > StaffID : VARCHAR(6),
    >
    > StaffName : VARCHAR(40)
    >
    > )

- Changing Table Definition

  - > ALTER TABLE STAFF
    >
    > ADD YearService INTEGER ;

- Adding Primary Key to Table

  - > CREATE TABLE LOCATION
    >
    > (
    >
    > CITY NOT NULL;
    >
    > CITY : VARCHAR(6),
    >
    > PRIMARY KEY (CITY);
    >
    > )



### Data Manipulation Language

- Queries

  - > SELECT

  - > FROM 

  - > WHERE

  - > ORDER BY

  - > GROUP BY

  - > INNER JOIN

- Queries - From Two Tables

  - > INNER JOIN

- Data Maintenance

  - > DELETE

  - > UPDATE

  - > INSERT INTO

  - > FROM

- 







