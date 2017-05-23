![GitHub Logo](https://s3.ap-south-1.amazonaws.com/greyatom-social/GreyAtom-logo.png)

# Key Challenges

### Relational Databases Are Not Designed For Scale

* Relational databases are designed to run on a single server in order to maintain the integrity of the table mappings and avoid the problems of distributed computing.
* Achieving scalability and elasticity is a huge challenge for relational databases. Relational databases were designed in a period when data could be kept small, neat, and orderly. That’s just not true anymore. Yes, all database vendors say they scale big. They have to in order to survive. But, when you take a closer look and see what’s actually working and what’s not, the fundamental problems with relational databases start to become more clear.

<br />

### New Architectural Changes Only Hide the Underlying Problem
* To handle these concerns, relational database vendors have come out with a whole assortment of improvements. Today, the evolution of relational databases allows them to use more complex architectures, relying on a “master-slave” model in which the “slaves” are additional servers that can handle parallel processing and replicated data, or data that is “sharded” (divided and distributed among multiple servers, or hosts) to ease the workload on the master server.
* The enhancements to relational databases also come with other big trade-offs as well. For example, when data is distributed across a relational database it is typically based on pre-defined queries in order to maintain performance. In other words, flexibility is sacrificed for performance.

<br />

### Transaction Support
* When we start distributing data, the consistency among the distributed data store becomes an issue.

<br />

### Workload and Usage Profile
* New application requires high availability and low latency ex. web application and mobile application
* The need for ACID is not very important why pay the price?
* Write once and read multiple times
* New data type: Image, Video, files, etc.
* Structured differently, XML, JSON, etc.

<br />

### NoSQL Databases are Designed for Scale
* Rather than be constrained by the limits of single-server architectures, NoSQL databases are designed for massive scale on distributed systems (usually hundreds of Terabytes rather than tens of Gigabytes). They can scale-out “horizontally,” meaning that they run on multiple servers that work together, each sharing part of the load.
* Massive scale is impressive, but what is perhaps even more important is elasticity.
