# Glossary of Terms

## Databases
| Terminology          | Definition                                                |
|----------------------|-----------------------------------------------------------|
| Attribute            | A column                                                  |
| Tuple                | A row                                                     |
| Domain               | Allowable values                                          |
| Atomic Data          | Data that cannot be broken down any further               |
| Compound Primary Key | A priamry key made up of more than one attribute          |
| 1 Normal Form (1NF)  | Remove repeating and multivalued attributes               |
| 2 Normal Form (2NF)  | Remove partially dependant attributes and non-key attributes depend on all of the primary key |
| 3 Normal Form (3NF)  | There are no non-key attributes that depend on another non-key attribute (transitive) |
| Foreign Key          | A field in a table that uniquely identifies a row in another table |
| Primary Key          | A field that indentifies all table records |
| TERMINOLOGY HERE | DEFINITION HERE |

## Complex stage of Normalisation
### Unnormalised Data#
|first name|last name|email|telephone1|telephone2|location|
|---|---|---|---|---|---|
|John|Doe|johndoe@example.com|01120434999|08475357483|UK|

| first name | last name | full name |  | location |
|------------|-----------|-----------|-------|----------|
| John       | Doe       | John Doe  | a@b.c | Ohio     |

### Normal Form 1
* Removed first name and last name
* Created second table for departments

| id | full name | email | location |
|----|-----------|-------|----------|
| 0  | John Doe  | a@b.c | Ohio     |

## Normalisation simplified
* First Normal Form - The information is stored in a relational table and each column contains atomic values, and there are not repeating groups of columns.
* Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
* Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key.
