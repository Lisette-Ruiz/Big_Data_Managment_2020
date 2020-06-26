***
## 1. What is Log  used for it is usefull in databases?.

- The word log is often used to refer to application logs, where an application outputs text that describes what’s happening.
- log is used in the more general sense: an append-only sequence of records. 

**Note**: It doesn’t have to be human-readable; it might be binary and intended only for other programs to read.



***

## 2. **In chapter 3 it is described that db_get has terrible performance, why?**
- There is a problem if you have a large number of records in your database, since every time you want to look up a key, db_get has to scan the entire database file from beginning to end, looking for occurrences of the key.

**Note**: In algorithmic terms, the cost of a lookup is O(n): if you double the number of records n in your database, a lookup takes twice as long. 
 
***

## 3. **Describe what "compaction" mean,  focussing on key values.**

Compaction means throwing away duplicate keys in the log, and keeping only the most recent update for each key.In other words, it is the compaction of a key-value update log (counting the number of times each cat video was played), retaining only the most recent value for each key.


***

## 4. **Explain the difference between Transaction processing and batch processing **
- Transaction processing
just means allowing clients to make low-latency reads and writes; as opposed to batch processing jobs, which only run periodically (for example, once per day).

***

## 5. Why is it said that databases started to be used for data analysis?

- Because when returning the query data, they are requested with certain operations or are filtered. an analytical query should be scanned over a large number of records, (only reads a few columns per record) and computes aggregated statistics (such as count, sum, or average) instead of returning raw data to user.


