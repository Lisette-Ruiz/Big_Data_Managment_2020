***
## 1. What does atomicity refer to and what does it do?

R: That can be better understood as abortability. If a transaction was aborted, the application can be sure that it didn't change anything, so it can safely be retried.


***

## 2. Based on the idea that databases only store information, how could you make the data meet certain specifications?
R: Using foreign key constraints or unique constraints.

 
***

## 3. What is the central idea of ACID consistency and on what does it depend?

R:
.The idea of ACID consistency is that you have certain statements about your data (invariants) that must always be true.
-It depends on the application’s notion of invariants.

***


## 4. Imagen two clients simultaneously incrementing a counter that is stored in a database. Each client will read the current value, add 1, and write the new value back; the counter normally should have increased from 42 to 44, However it got 43 because of the race condition. that the owner of ACID would take care of that situation and why. 

R: Isolation-Serialization.
Since each transaction can pretend that it is the only transaction running on the entire database. It means that concurrently executing transactions are isolated from each other: they cannot step on each other’s toes.

***

## 5. What does Durability in ACID refer to?

R: Durability is the promise that once a transaction has committed successfully, any data it has written will not be forgotten, even if there is a hardware fault or the database crashes.

***

## 6. Formulate and explain a simple concurrency problem

R. Multiple clients accessing the same record in a database at the same time. (race conditions)
