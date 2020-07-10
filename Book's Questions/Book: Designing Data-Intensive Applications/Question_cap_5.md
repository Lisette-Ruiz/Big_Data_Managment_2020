***
## 1. Why is it important to keep a copy of the same data on multiple machines that are connected through a network?

- To keep data geographically close to your users (and thus reduce latency).
- To allow the system to continue working even if some of its parts have failed
(and thus increase availability).
- To scale the number of machines that can serve reading queries (and therefore
increase reading performance).


***

## 2. Describe what a simultaneously constant automatic failover process consists of in the following steps.
- Determining that the leader has failed.
- Choosing a new leader.
- Reconfiguring the system to use the new leader.
 
***

## 3.Explains what is log log for a relational database and describes some of its properties described in chapter 5

It is usually a sequence of records that describe writes to database tables with the granularity of a row.

- For an inserted row, the record contains the new values of all the columns.

- For a deleted row, the record contains enough information to uniquely identify the row that was deleted. Normally, this would be the primary key, but if there is no primary key in the table, the old values of all columns should be recorded.

- For an updated row, the record contains enough information to uniquely identify the updated row and new values for all columns (or at least new values for all columns that changed).

***


## 4. In solutions for Replication Lag, what are transactions?
- They are a way for a database to provide stronger guarantees so that the application can be simpler.

***

## 5.  Compare how the single-leader and multi-leader configurations fare in a multidatacenter deployment:

- Performance

In a single-leader configuration, every write must go over the internet to the datacenter with the leader. While In a multi-leader configuration, every write can be processed in the local datacenter and is replicated asynchronously to the other datacenters. 

- Tolerance of datacenter outages
In a single-leader configuration, if the datacenter with the leader fails, failover can promote a follower in another datacenter to be leader. In a multi-leader configuration, each datacenter can continue operating independently of the others, and replication catches up when the failed datacenter comes back online.

- Tolerance of network problems
A single-leader configuration is very sensitive to problems in public internet interdatacenter link, because writes are made synchronously over this link. A multi-leader configuration with asynchronous replication can usually tolerate network problems better: a temporary network interruption does not prevent writes being processed.

***

## 6. which is the simplest strategy for dealing with conflicts,  please justify your answer.

The simplest strategy for dealing with conflicts is to avoid them: if the application can ensure that all writes for a particular record go through the same leader, then conflicts cannot occur.
