---
title: Database Research
tags: db, research
---


    “What I cannot create, I do not understand.” – Richard Feynman

## People && Group

### Group
* [MIT db](http://db.lcs.mit.edu/)
* [CMU db](http://db.cs.cmu.edu/)
* [UCB db](http://db.cs.berkeley.edu/)
* [Stanford infolab](http://infolab.stanford.edu/)
* [Stanford dawn](http://dawn.cs.stanford.edu/)
* [UW-Madison db](https://database.cs.wisc.edu/)
* [UW db](http://db.cs.washington.edu/)
* [UMich](http://dbgroup.eecs.umich.edu)
* [Yale db](http://db.cs.yale.edu)

### People

* Joe Hellerstein
>  group : [UCBdb](https://db.cs.berkeley.edu)
[website](https://db.cs.berkeley.edy/jmh/)
[blog](https://databeta.wordpress.com)
[github](https://github.com/jhellerstein)

* Andy Pavlo : 
>  group : [CMUdb](http://db.cs.cmu.edu/)
[website](http://www.cs.cmu.edu/~pavlo)
[blog](http://www.cs.cmu.edu/~pavlo/blog/index.html)
[github](https://github.com/apavlo)

* Peter Balis : 
>  group : [Stanford dawn](http://dawn.cs.stanford.edu), [Stanford         FutureData](http://futuredata.stanford.edu/)
[website](http://www.bailis.org/)
[blog](http://www.bailis.org/blog/)
[github](https://github.com/pbailis)

* Daniel Abadi :
>   [website](http://www.cs.umd.edu/~abadi/)
[blog](http://dbmsmusings.blogspot.com/)
[github](https://github.com/abadid)





## Paper
* [A common database approach for OLTP and OLAP using an in-memory column database, Sigmod09](https://dl.acm.org/citation.cfm?id=1559846)

* [Middleware-based database replication: the gaps between theory and practice, Sigmod08](https://dl.acm.org/citation.cfm?id=1376691)

* [Column-stores vs. row-stores: how different are they really?](https://academic.microsoft.com/#/detail/2005112390)

## Project
### Relations Database Management System

* [Hekaton](https://www.microsoft.com/en-us/research/publication/hekaton-sql-servers-memory-optimized-oltp-engine/)
> Hekaton is a memory-optimized OLTP engine integrated in SQL Server 2014 and is also known as The In-Memory OLTP. Hekaton allows a table to be stored and resides in main memory and can be queried in the same way as disk-based SQL Server tables. Hekaton mainly improves its performance on many-core CPUs by improving scalability and reducing the number of instructions executed for a single query. Scalability is provided by Hekaton by eliminating latches and locks. Native compilation process which compiles stored procedures and tables into efficient machine code can reduce instructions executed for queries.]

* [Calvin](http://github.com/yaledb/calvin)
> Calvin is a scalable transactional database system that leverages determinism to guarantee active replication and full ACID-compliance of distributed transactions without two-phase commit. Most of the code is for VLDB 2014 paper: 《An Evaluation of the Advantages and Disadvantages of Deterministic Database Systems》

* [Yugabyte](https://github.com/YugaByte/yugabyte-db)
> YugaByteDB is a transactional, high-performance database for building distributed cloud services. It supports Cassandra-compatible and Redis-compatible APIs, with PostgreSQL in Beta. 

* [Hyrise](https://hpi.de/plattner/projects/hyrise.html)
> in-memory storage engine Hyrise

* [Zero](https://github.com/caetanosauer/zero)
> Zero is a transactional storage manager used mainly for prototyping in Database Systems research. It supports operations on a Foster B-tree data structure with ACID semantics. Zero is designed for highly scalable, high-throughput OLTP. Being a research prototype, it does not provide certain usability features expected on a real production-level system.

* [Yesquel](https://www.yesquel.org)
	* [Github, yesquel](https://github.com/mkaguilera/yesquel)

* [Shore-mt](https://sites.google.com/site/shoremt/home)
>Shore-MT is an experimental test-bed library to be used by researchers who are interested in pursuing research on multi-threaded software that manages persistent data. Shore-MT as a storage engine provides the following capabilities:


* [DBx1000](https://github.com/yxymit/DBx1000)
> DBx1000 is an single node OLTP database management system (DBMS). The goal of DBx1000 is to make DBMS scalable on future 1000-core processors. We implemented **all the seven classic concurrency control schemes** in DBx1000. They exhibit different scalability properties under different workloads.
The concurrency control scalability study is described in the following paper.
Staring into the Abyss: An Evaluation of Concurrency Control with One Thousand Cores
Xiangyao Yu, George Bezerra, Andrew Pavlo, Srinivas Devadas, Michael Stonebraker
http://www.vldb.org/pvldb/vol8/p209-yu.pdf


* [Deneva](https://github.com/mitdbg/deneva)
> DDBMS
DDBMS is a testbed of an OLTP distributed database management system (DBMS). It supports 6 concurrency control algorithms.
This testbed is based on the DBx1000 system, 


* [Cavalia](https://github.com/cavalia/cavalia)
> A transactional main-memory database on multicores.
Features
Cavalia is a main-memory database system specifically designed for modern multicore architectures. It aims at providing a generalized framework for comparing different concurrency-control mechanisms. A highlight in Cavalia is that new hardware features (e.g., NUMA, HTM, and NVRAM) are judiciously leveraged for achieving higher level of concurrency when processing massive volume of transactions.
Disclaimers
Our project aims at faithfully implementing all kinds of concurrency-control and failure-recovery schemes in the same database framework.

* [Silo](https://github.com/stephentu/silo)
> This project contains the prototype of the database system described in
Speedy Transactions in Multicore In-Memory Databases 
Stephen Tu, Wenting Zheng, Eddie Kohler, Barbara Liskov, Samuel Madden 
SOSP 2013. 
http://people.csail.mit.edu/stephentu/papers/silo.pdf


* [Peloton](https://github.com/cmu-db/peloton)
> What Is Peloton?
A self-driving SQL database management system.
Integrated artificial intelligence components that enable autonomous optimization.
Native support for byte-addressable non-volatile memory (NVM) storage technology.
Lock-free multi-version concurrency control to support real-time analytics.
Postgres network-protocol and JDBC compatible.
High-performance, lock-free Bw-Tree for indexing.
100% Open-Source (Apache Software License v2.0).


* [H-Store](http://web.archive.org/web/20171213185648/http://hstore.cs.brown.edu/)
> H-Store is an experimental main-memory, parallel database management system that is optimized for on-line transaction processing (OLTP) applications. It is a highly distributed, row-store-based relational database that runs on a cluster on shared-nothing, main memory executor nodes.

* [C-Store](http://db.lcs.mit.edu/projects/cstore/)
> C-Store is a read-optimized relational DBMS that contrasts sharply with most current systems, which are write-optimized. Among the many differences in its design are: storage of data by column rather than by row, careful coding and packing of objects into storage including main memory during query processing, storing an overlapping collection of column-oriented projections, rather than the current fare of tables and indexes, a non-traditional implementation of transactions which includes high availability and snapshot isolation for read-only transactions, and the extensive use of bitmap indexes to complement B-tree structures. 

* [ClickHouse](https://github.com/yandex/ClickHouse)
> ClickHouse is an open source column-oriented database management system capable of real time generation of analytical data reports using SQL queries.


* [Postgresql-cpp](https://github.com/jarulraj/postgresql-cpp)
> transplant postgresql into C++

* [Hyper](http://hyper-db.de/)
> HyPer is a main-memory-based relational DBMS for mixed OLTP and OLAP workloads. It is a so-called all-in-one New-SQL database system that entirely deviates from classical disk-based DBMS architectures by introducing many innovative ideas including machine code generation for data-centric query processing and multi-version concurrency control, leading to exceptional performance. HyPer’s OLTP throughput is comparable or superior to dedicated transaction processing systems and its OLAP performance matches the best query processing engines — however, HyPer achieves this OLTP and OLAP performance simultaneously on the same database state. Current research focuses on extending HyPer’s functionality beyond OLTP and OLAP processing to exploratory workflows that are deeply integrated into the database kernel by utilizing HyPer’s pioneering compilation infrastructure.

* [database vertical partitioning](https://github.com/palatinuse/database-vertical-partitioning)

## Courses
### concept
- [Introdution to Database, Stanfordcs145](https://cs145.stanford.edu)

### implementation
- [Introduction to Database Systems, CMU15-445](https://15445.cs.cmu.edu)

- [Database Systems, MIT6.830](https://db.csail.mit.edu/6.830)

### advanced topic
- [Advanced Database Systems, CMU15-721](http://15721.courses.cs.cmu.edu)

- [Advanced Topics in Database Systems, CMU15-799](http://www.cs.cmu.edu/~pavlo/courses/fall2013/)

### distributed database
- [Distributed Database Systems, PurdueCS542](https://www.cs.purdue.edu/homes/clifton/cs542/),   [Spring 2016](https://www.cs.purdue.edu/homes/bb/cs542-16Spr/)

- [Distributed Database Systems, Thu-Cmu](http://thu-cmu.cs.tsinghua.edu.cn/curriculum/ddb_website)

- [Parallel and Distributed Database Systems
(Winter 2013), UWaterlooCS742](https://cs.uwaterloo.ca/~tozsu/courses/CS742/W13/index.html)


## Reference
* [Let's build a simple database](https://cstack.github.io/db_tutorial/)
* [The nuts and bolts of DBMS construction: building your own prototype](http://pages.saclay.inria.fr/ioana.manolescu/SLIDES/LernerManolescu-SBBD2003.pdf)
* [Building a new database management  system in acadimia](http://www.cs.cmu.edu/~pavlo/blog/2017/03/building-a-new-database-management-system-in-academia.html)
* [The last decade of database research and its blindingly bright future. or Database Research: A love song](https://dawn.cs.stanford.edu/2018/04/11/db-community/)






