 

# IN-MEMORY DATABASE {#cabecera1}
[**Main memory database or MMDB**](#cabecera1)

***

### What In-memory Databases Are For? 

: In-memory databases are designed to achieve minimal response time by eliminating the need to access disks. Because all data is stored and managed exclusively in main memory, you risk being lost in a process or server failure. In-memory databases can preserve data on disks by storing each operation in a log or taking snapshots. 

 - - -

### In-memory are made for: 

: In-memory databases are ideal for applications that require microsecond response times and can have large spikes in traffic at any time, such as game leaderboards, session stores, and real-time analytics. 

 ***

### Properties of In-memory Database Systems 

- **Atomicity** : this involves a single data transfer and avoids the optimized processing of multiple data transfers. Every transaction is "all or nothing". 
- **Consistency**: This ensures that the data exists in a consistent and valid state that complies with all defined data existence rules. 
- **Isolation**: It ensures that each transaction runs in total isolation and is completely independent of any other concurrent transactions. 
- **Durability**: It ensures the completion of a transaction once assigned, even in the event of power loss, crashes, or errors. 

 - - -

### Advantages of In-memory Database Systems.

1. An in-memory database system streamlines processing by eliminating multiple data transfers, reduces memory consumption by removing multiple copies of data, and simplifies processing by minimizing CPU demands. 

2. __The major advantage of systems using in-memory databases vs traditional database systems is: its performance speed.__ 

3. Source data is loaded into the system memory in a compressed and  format. Therefore, in-memory processing reduces disk seek time for accessing data and streamlining the work involved in processing queries. 

4. The internal optimization algorithms for in-memory databases are simpler and execute fewer CPU instructions, thereby facilitating faster response times than disk-optimized databases. 

***

## IN-MEMORY DATABASES.

Comparation between 4 in-memory databases:

 F   | Redis | Kinetica | Apache Ignite | Oracle RDBMS 
-- | -- | -- | -- | -- |
**Client interface** | C, C++, Python, Lua, C# | C++, C#, Java, JavaScript, Node.js. Python, HTTP | Java, SQL, JDBC, ODBC | F 
**License** |	Open Source (BSD) | Proprietary | Open Source (Apache License Version 2.0) | Proprietary
**Best Used** | Resolve very complex programming problems with simple commands executed within the data store, reducing coding effort, increasing throughput, and reducing latency. | Kinetica is an ideal solution for data discovery projects. | It was designed to store and compute on large volumes of data across a cluster of nodes.| It provides database introspection and various instruments for creating and modifying objects for the supported engines.
**Main focus** | It scales horizontally and provides ACID transactions. | An analytics platform designed to handle extremely large and complex datasets with ease. | Scaled horizontally, it distributes key-value pairs across the cluster. Data is rebalanced every time a node is added/removed from the cluster. | First database designed for enterprise grid computing. the most flexible and cost-effective way to manage information and applications
**Acronym**  | Remote Dictionary Server | f  | F | Oracle Relational database management system.
**Developer** | Redis Labs | Kinetica (formerly GIS Federal) | Apache Software Foundation, GridGain Systems | Oracle Corporation
**Consistency** | It is networked, in-memory, and stores keys with optional durability. | Functions like a RDBMS (structured data) for fast analytics on datasets in the hundreds of GBs to 10's of TBs range. | Durable, strongly consistent, and highly available with powerful SQL, key-value and processing APIs. | RDBMS Oracle 12c contains an option for in-memory technology (additional licenses required).
**Platforms** | Written in ANSI C and works in most POSIX systems like Linux, *BSD, OS X. | GPU-Accelerated Database. | Apache is a platform designed to store and compute on large volumes of data across a cluster of nodes. | Make market-leading components (databases, application servers, web servers, which lets customers to implement PeopleSoft on the infrastructure.






