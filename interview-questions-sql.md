Interview Questions -- SQL
==========================

**Explain about Delete vs Truncate vs Drop.**

**Delete**

	- can delete one record.
	- can delete all records at the same time.
	- table structure will be in the database even though all records got deleted.
	- can rollback after delete operation.
	- delete operation is slower than drop, truncate.
 
**Truncate**

	- can not truncate one record.
	- can truncate only all records at the same time.
	- table structure will be in the database even though all records got truncated.

**Drop**

	- can not drop one record.
	- can drop only all records at the same time.
	- table structure will not be in the database when the table got dropped.
	- can not rollback after drop operation.
	- drop operation is faster than delete.

**Explain Primary key and Foreign Key in detail.**

**PK (Primary key)**

The primary key uniquely identifies each record in a table.

	- primary key has to be unique
	- it can not repeat
	- can not have a null value
	- a table can have only one PK

**FK (Foreign Key)**

A foreign key in one table points to a primary key in another table

	- FK can have null values
	- in one table we could have multiple FK
	- FK values can be repeated

