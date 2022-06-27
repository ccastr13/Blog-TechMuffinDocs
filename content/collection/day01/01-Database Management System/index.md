---
date: "2022-06-23"
draft: false
excerpt: First article
subtitle: Examples of database systems, drawbacks, and architecture.
title: Database Management System
weight: 1
---
## Database Management System
A database management system (DBMS) is a collection of related data a set of programs to access those datasets. It is a logical grouping of data categorized according to their data structures or types.

Similar to a physical filing cabinet. You have folders logically grouped together based on categories. The filing cabinet is the database and the folders are the tables. 


### Examples of Database Applications
A real-world example of a database management system is every social media site from Facebook to Tik Tok. They store an abudance of user information to recommend products to you the consumer. The type of databases the social media companies use varies from NoSQL  databases or MySQL. Nonetheless, database management systems allow data to always be accessible and easily deilverable.

More Examples:
  - Healthcare
  - eCommerece
  - Video Streaming
  - Finances


### Drawbacks of file systems to store data
While there are advantages of a file-oreiented system there are still drawbacks

1. Data Inconsistency and redundancy
    - It is possible for data to be dupilicated in different filess leading to data redundancy and resulting in memory wastage
2. Difficulty in accessing data
    - The data tends to be isolated
    - Integrity Problem/constraints e.g. balance > 0
3. Atomicity of updates
    - This is required to save data values. Any system can fail at any time and as such the the data should be in a consistent state. Actions should happen all together or not at all.
4. Concurrent access by multiple users
    - Multiple users are allowed to access data simultaneously. This is for the sake of better performance and faster response.
5. Security problems
    - Not every user of the database system should be able to access all data. Each use should be allowed to access data concerning their requirements only.


  Still in spite of so many disadvantages, File Processing System is still good for small organizations because it does not require costly softwares and programmers to handle it.


## An Architecture for DBMS
The ANSI-SPARC database architecture is the bases of most modern databases.

There are 3 levels:
1. Physical Level
1. Logical Level
3. External Level

<img src="Architecture for DBMS.png" width="400"/>

<br/>

### Physical Level
Describes how records or data are stored, and describes the data structures used by the database.

### Logical Level
Describes the data stored in the Database and the relationships between various data tables. 

### External Level
Contains the application programs to hide details of data. It only shows the relevant database content to users in the form of views. Each view is a window to see certain information about the data.

<br/>

## Schema and Instance

**Schema** - the logical structure of the database (overall design)  <br />
**Instance** - actual content of the databse at a particular point in time


## Data Models
  - A collection of tools for describing
    - data
    - data relationships
    - data semantics
    - data constraints
   
   ex: Relational Model
      - a collection of tables to represent data and relationships

Refrences:

1. https://tutorialink.com/dbms/advantage-and-disadvantages-of-file-oriented-system.dbms#:~:text=Disadvantage%20of%20File-oriented%20system%3A%201%20Data%20Redundancy%3A%20It,allowed%20to%20access%20data%20concerning%20his%20requirements%20only.

2. https://whatisdbms.com/disadvantages-of-file-processing-system/

3. https://www.tutorialspoint.com/Three-levels-of-database-architecture
  
