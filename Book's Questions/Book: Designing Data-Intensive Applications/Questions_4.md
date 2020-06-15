
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

## 3. Describe the three rules to “normalization” a database, better known as “Normal form”:
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

## 4.What is the advantage of using an identification (ID):

- It is that since it has no meaning to humans, it never needs to change: the ID can stay the same, even if the information it identifies changes.

***

## 5. What is the network model and why is it known as CODASYL model?

The CODASYL model was a generalization of the hierarchical model. In the tree structure of the hierarchical model, each record has exactly one parent; in the network model, a record could have multiple parents.
>> e.g:
> For example, there could be a record for the "Greater Seattle Area" region, and all users who lived in that region could be linked to it. This enabled many-to-one and many-to-many relationships to be modeled.

***

## 6. Describe if there is a query language paradigm for each specific use case and describe what you should consider before choosing one?

No, it simply adapts to the need. Neither paradigm is better than the other; each has different strengths for software development.

### Aspects to consider before choosing a query language paradigm:
- The project requires greater precision and control.
- Imperative query languages ​​work well.
- If speed and productivity of the development process are more important, declarative languages ​​offer the flexibility to get results without much effort.

***
