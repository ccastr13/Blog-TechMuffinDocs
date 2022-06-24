---
date: "2021-01-02"
draft: false
excerpt: Grid is the very first CSS module created specifically to solve the layout
  problems we’ve all been hacking our way around for as long as we’ve been making
  websites.
subtitle: The following are the shapes and lines used to create ER diagrams that are then translated to table structure.
title: ER Diagram Symbols, Relationships and Cardinality
weight: 3
---
# Definition
An Entity Relationship Diagram (ERD) is a type of structural diagram for use in database design. An ERD shows the major entities within the system scope, and the inter-relationships among these entities.

<br/>

# Symbol and Notations
The following are the symbols utiliezed in ERDs:

<br/>

Entity Type

<img src="ER Diagram - Entity Type.png" width="100"/>

<br />

Attributes

<img src="ER Diagram - Attributes.png" width="500"/>

<br />

Example of Entity Type with Attributes

<img src="ER Diagram - Example.png" width="500"/>

<br />

Relationship Type

<img src="ER Diagram - Relationship.png" width="200"/>

<br />

Example with Relationship Type

<img src="ER Diagram - Example with Attributes.png" width="500"/>


<br />


# Cardinality Constraint

## Types of Cardinality:
- One to One 1:1

- One to Many 1:N

- Many to One N:1

- Many to Many N:M

<br />

### One to One
An entity in A is associated with at most one entitiy in B
An entity in B is associated with at ost one entitiy in A

<br/>

### One to Many
<insert diagram>

<br />

### Many to Many
<Insert Diagram>

<br />

# Structural Constraints
- Cardinality
- Participation constraint
  - The existence dependency of an entitiy on it's participation in a relationship instance

## Total Participation
e.g. an amployee must work in a department

<insert diagram>

<br />

## Partial Participation

<insert diagram>

<br />

## Min/Max Pairs

0 <= min
min <= max

min = 0         Partial Participation
min > 0         Total Participation

<br />

# Keys

*Super Keys* - A set of one or more attributes identifies each entitiy uniquely in its enetitiy type

e.g. Student entitiy
      {sID}, {name, DoB, address}

*Candidate Keys* - A super key for which no proper subset is a super key

e.g.
      {sID, name} &rarr; super key

      {sID, name} >={sID} &larr; super key
      {sID} is a proper subet of {SID, name}

      {sID, name} &rarr; not a candidate key
      {sID} &larr; is candidate key

*Primary Key* - A candidate key that is chosen by the DBA as the principle means of identifying entities

Primary Key Attributes are underlined in ER Diagram

<inset diagram>
