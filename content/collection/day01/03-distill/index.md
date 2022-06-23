---
date: "2021-01-02"
draft: false
excerpt: Grid is the very first CSS module created specifically to solve the layout
  problems we’ve all been hacking our way around for as long as we’ve been making
  websites.
subtitle: Using the distill & postcards packages to build a personal website with
  R Markdown.
title: ER Diagram Legend
weight: 3
---

## ER Diagram

**Entity Type**

<img src="ER Diagram - Entity Type.png" width="200"/>


**Attributes**

<img src="ER Diagram - Attributes.png" width="500"/>


## Relationship Type
<insert diagram image>


## Cardinality Constraint
One to One 1:1
One to Many 1:N
Many to One N:1
Many to Many N:M


# One to One

<insert diagram>

An entitiy in A is associated with at most one entity in B
An entity B is associated with at most one entitiy in A

# One to Many
<insert diagram>

# Many to Many
<Insert Diagram>

## Structural Constraints
- Cardinality
- Participation constraint
  - The existence dependency of an entitiy on it's participation in a relationship instance

# Total Participation
e.g. an amployee must work in a department

<insert diagram>

# Partial Participation

<insert diagram>

# Min/Max Pairs

0 <= min
min <= max

min = 0         Partial Participation
min > 0         Total Participation

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
