---
date: "2021-01-02"
excerpt: 
subtitle: The design process,query language, and ER models.
title: Database Development Process
weight: 2
---

## Database Development Process
The Database Devepment Pricess is a cycle as such developers are able to cycle back to phases based on adjustments needs. The following are the steps taken when designing a database:

1. Feasibility Analysis
    - Determines what needs to be done, clarifies the scope, and considers the cost, time, and need for the system.

2. Requirements Collection & Analysis
    - A coneptual data model is created based on the data analysis of the data requirements statement.
    - This data includes selection of database goals and establishment of the requirements for hardware and software.
    - In sume the requirement analysis consits of 
      - Figuring out a problem and its analysis;
      - Statement of requirements.

3. Design
    - Database design is a substantial part of database development. The full database development cycle includes its conceptual, logical and physical design. The main goals at this stage are:
      - Specificy the structure of the information system
      - Database design and application design

4. Implementation
    - In this phase the DBMS is installed on the required hardware, database is created, and the data is loaded. THen the security of the database is set up at this stage, the system is tested, and users are given according to their requirements.
    - In sum this phase consists of:
      - Construct database and populate it w/ data
      - Develop application programs

5. Validation and Acceptance Testing

6. Operation
  - Once the database is implemented the operation phase of the database system begins. This consists of monitoring and maintaining the database system. Maintenance includes activities such as adding new fields, changing the size of existing file, correcting any problems, and implementing other enhancements


## Database Design Process
- ER (Entry-Relation) Model
- Transaction Design
  - Input/output description
  - Functional behavior retrieval transaction update
- Semi-structured data Model XML

<br/>

# Data Manipulation Language (DML)
- Languages for accessing and manipulating data organized by data model
- Insert/Delete/Retrieve/Modify Data


## Query Language
- Query: the retrievl of information
  ex) SQL (Structured Query Language)
  
  
## Data Definition Language (DDL)
- Specificy the database schema
ex) 

```
create table (
  ID char(5)
  Name varchar(10)
  Dept varchar(5)
  )
```
> Note: char = 5 and varchar<10

<br/>

**Student**
| ID      | Name | Dept
| ----------- | ----------- |----------- |
| 1111      | AA       | CS
| 2222   | BB        | EE


<br/>

## Data Dictionary
- Stores meta data
  - Database Schema
  - Integrity Constraint
  - Authorization



## Entry-Relationship (ER) Conceptual Model

### Entitiy Type
- An object that exists and is distinguishable from other objects e.g.) student, company
- Represented by a set of attricbutes
  - ex) student  &rarr; id, name, address

> Note: Entities must contain attribute(s)

### Entitiy Set
- A set of entities of the same type

**Student**
| ID      | Name | 
| ----------- | ----------- |
| 1111      | Brown       |
| 2222   | Chavez        |

<br>

### Relationship Set
- A set of relationships of the same type

**Student**
| ID      | Name | 
| ----------- | ----------- |
| 1111      | Brown       |
| 2222   | Chavez        |

**Course**
| Name      | Title | 
| ----------- | ----------- |
| CSE310      | Data Stuctures and Algorithsm|
| CSE412   | Database Management|

<br/>

e.g.) (1111, CSE310)
      (2222, CSE412)
      
{(e<sub>1</sub>, e<sub>2</sub>,..., e<sub>n</sub>) | e<sub>1</sub> member of E<sub>1</sub>, e<sub>2</sub> member of E<sub>2</sub>, e<sub>n</sub> member of E<sub>n</sub>} where (e<sub>1</sub>, e<sub>2</sub>,..., e<sub>n</sub>) is a relationship


Refrences
1. https://wofford-ecs.org/DataAndVisualization/DatabaseDevelopment/material.htm#:~:text=The%20relational%20database%20lifecycle%20is%20the%20process%20of,the%20project%20be%20approved%2C%20system%20requirements%20are%20collected.
2. https://joinsoft.com/blog/database-development-process-steps/
3. https://zitoc.com/phases-in-database-development-process/