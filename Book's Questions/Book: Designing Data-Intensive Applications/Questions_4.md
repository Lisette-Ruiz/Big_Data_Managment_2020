
***
## 1. Name of the rule or method that allows reducing the amount of repetitive code required in SQL and which mentions some of its requirements.

- Normalization.

 **Requirements:**
- Each table must have a unique name.
- There can not be two equal rows.
- Duplicates are not allowed.
- All data in a column must be of the same type.

***
## 2. **What is known as independence misadjustment?**
- To disconnect database models of tables, rows and columns
 
***
## 3. Describe the 3 rules to “normalization” a database, better known as “Normal form”:
> First normal form
- Delete the repeating groups from the individual tables.
- Create a separate table for each related data set.
- Identify each set of data related to a primary key.
> Second normal form
- Create separate tables for sets of values that apply to multiple records.
- Relate these tables to a foreign key.
> Third normal form
- Delete the fields that do not depend on the key.
***
