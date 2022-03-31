---
date: "2021-01-01"
draft: false
excerpt: How to prepare ahead of time.
subtitle: ""
title: Prework
weight: 1
---

Welcome to the [Introducing Yourself Online](/) workshop! We look forward to meeting you. Before attending the workshop, please complete the following prework.

## Set up RStudio Cloud

Sign up for a free RStudio Cloud account at https://rstudio.cloud/ before the workshop. I recommend logging in with an existing Google or GitHub account, if you have one (rather than creating a new account with another password you have to remember). I want you to be able to work from your own laptop in this workshop, but Cloud is an important back-up plan should you run into troubles.

## Set up GitHub

We will be using GitHub in this workshop for version control and publishing. Sign up for a free GitHub.com account at <https://github.com/join> if you don't already have one. Also:

+ Complete these [installation instructions](https://happygitwithr.com/install-intro.html).
    
+ Test your connection between GitHub and RStudio following [these steps](https://happygitwithr.com/connect-intro.html). 
    
+ **NOTE:** We *strongly recommend* that if you are not already a fluent GitHub user you choose [HTTPS over SSH](https://happygitwithr.com/credential-caching.html).

## Brush up on markdown

Please complete this [10-minute interactive tutorial on Markdown](https://commonmark.org/help/tutorial/). 

## Installations

Please bring a laptop that has the following installed:

+ A recent version of R (>=3.6.0), which is available for free at https://cloud.r-project.org/
    
+ A recent version of RStudio Desktop (>=1.4), available for free ([RStudio Desktop Open Source License](https://www.rstudio.com/products/rstudio/download/#download)). Read up on the latest version [here](https://blog.rstudio.com/2021/01/19/announcing-rstudio-1-4/).
    
+ The R packages we will use, which you can install by connecting to the internet, opening RStudio, and running at the command line:

    ```r
    > install.packages(c("usethis", "remotes", "distill", 
                       "postcards", "blogdown"))
    ```
    
    You'll also need to install the development version of the `rmarkdown` package:
    
    ```r
    > remotes::install_github("rmarkdown")
    ```

## Install Hugo

To use blogdown, please install Hugo:
```r
> blogdown::install_hugo()
```

And ensure your current version is at least as high as:
```r
> hugo_version()
[1] ‘0.79.0’
```

## Check pandoc

The RStudio IDE bundles an updated version of pandoc- if you did install v1.4 of the IDE, you should be all set!

```r
> rmarkdown::pandoc_version()
[1] ‘2.11.3’
```


# Chapter 1

## Database Management System
A database management system (DBMS) is a collection of related data a set of programs to access those datasets.

### Examples of Database Applications
  - Balancing transactions
  - University, grades, registration

### Drawbacks of file systems to store data
  - Data Inconsistency and redundancy
  - Difficulty in accessing data
  - Data Isolation
  - Integrity Problem/constraints e.g. balance > 0
  - Atomicity ofupdates
    - actions should happen all together or not at all
  - Concurrent access by multiple users
  - Security problems
  -   Not every user of the database system should be able to access all data


## An Architecture for DBMS
<Insert image>

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
  
