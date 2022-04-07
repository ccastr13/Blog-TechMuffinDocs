---
date: "2021-01-02"
excerpt: In this block, we'll use the postcards package to make a single 'about' home
  page with only R Markdown.
subtitle: The design process,query language, and ER models.
title: Database Development Process
weight: 2
---

## Database Development Process
1. Feasibility Analysis
2. Requirements Collection & Analysis
3. Design
  a. Specificy the structure of the information system
  b. Database design and application design
4. Implementation
  a. Construct database and populate it w/ data
  b. Develop application programs
5. Validation and Acceptance Testing
6. Operation
  a. Train users
  b. maintencance


## Database Design Process
- ER (Entry-Relation) Model
- Transaction Design
  - Input/output description
  - Functional behavior retrieval transaction update
- Semi-structured data Model XML

## Data Manipulation Language (DML)
- Languages for accessing and manipulating data organized by data model
- Insert/Delete/Retrieve/Modify Data


# Query Language
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

**Student**
| ID      | Name | Dept
| ----------- | ----------- |----------- |
| 1111      | AA       | CS
| 2222   | BB        | EE


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

e.g.) (1111, CSE310)
      (2222, CSE412)
      
{(e<sub>1</sub>, e<sub>2</sub>,..., e<sub>n</sub>) | e<sub>1</sub> member of E<sub>1</sub>, e<sub>2</sub> member of E<sub>2</sub>, e<sub>n</sub> member of E<sub>n</sub>} where (e<sub>1</sub>, e<sub>2</sub>,..., e<sub>n</sub>) is a relationship
