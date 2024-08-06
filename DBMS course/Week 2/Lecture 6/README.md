# Data Definition Language
![](assets/Pasted%20image%2020240805204229.png)

# Domain Types in SQL
- `char(n)` - character with fixed size `n`
- `varchar(n)`- variable length with max size `n`
- `int`
- `smallint`
- `numeric(p,d)`- `p` number of total digits with `d` number of digits after the decimal point
- `real, double precision`
- `float(n)`- floating point number with atleast `n` digits

# Creating a table in SQL
- #### Syntax
	`create table <relation name> (A1 D1, A2 D2, A3 D3...)`
	where A and D are the attributes and domains respectively 
- Example
	`CREATE TABLE instructor (`
	`ID    char(5)`,
	`name   varchar(20)`
	`);`

# Integrity Constraints
We can add few constraints to make our program more logical and to avoid errors
- not null
- primary key($A_1, A_2...$)   {please note that primary keys cannot be null}
- foreign key($A_m.... A_n$) references r
Example:
![](assets/Pasted%20image%2020240805210415.png)
![](assets/Pasted%20image%2020240805210449.png)

This note suggests a modification to the primary key of the 'takes' table. Currently, the primary key includes (ID, course_id, sec_id, semester, year). By removing sec_id from this primary key, it would prevent a student from being registered in multiple sections of the same course in the same semester.

Here's why:

1. With sec_id in the primary key, a student could theoretically be registered for multiple sections of the same course in the same semester, as each combination would be unique.
2. By removing sec_id, the primary key would become (ID, course_id, semester, year). This ensures that for each student (ID), course (course_id), semester, and year combination, there can only be one record.
3. This change would enforce the rule that a student can only be registered for one section of a particular course in a given semester and year.

This modification helps maintain data integrity by preventing duplicate or conflicting course registrations for students.


# Updating tables in SQL
- ### Insert
	- ##### Syntax
		`INSERT INTO <relation name> VALUES ('32341', 'Rahul', 'Bio', 623243)`
		over here the tuple is inserted as per their order in the table and also in keeping with their domain
- ### Delete
	- ##### Syntax
		`DELETE FROM <relation name>`
		this deletes all the data in the relation table
- ### Drop table
	- ##### Syntax
		`DROP TABLE <relation name>`
		this makes it drop the entire table itself from the database
- ### Alter 
	- ##### Syntax
		`ALTER TABLE <relation name> ADD/DROP A D` where A is the new attribute and D is the new domain
		Note: for the already existing tuples for the new attribute the value will be null
		Note: many databases dont support `drop`


# Basic Query Structure


