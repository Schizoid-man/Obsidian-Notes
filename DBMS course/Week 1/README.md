## Levels of Abstraction
![Image 1](https://github.com/Schizoid-man/Obsidian-Notes/blob/c09a14c958ac1e3ed1c257f380a65a7c583c377d/DBMS%20course/Week%201/assets/Pasted%20image%2020240730124919.png)
![Image 2](https://github.com/Schizoid-man/Obsidian-Notes/blob/d146af5f33155c3dd7f0e9698afbbe6f0d6d751a/DBMS%20course/Week%201/assets/Pasted%20image%2020240730125617.png)

## Schemas and Instances
_Schema_ :_Basically an outline of the data required for our database_
We have 2 types: Logical Schema and Physical Schema
![Image 3](https://github.com/Schizoid-man/Obsidian-Notes/blob/da0c222d0562ed5befb13eb2c4dabe0b2dfeaf6f/DBMS%20course/Week%201/assets/Pasted%20image%2020240730125945.png)
The schemas only tell us about the type of data stored in it. It is just a container or a label for the data. It **isn't the actual data itself stored in the database.**

_Instances_ : The actual data stored in the database is the instance. 

![Image 4](https://github.com/Schizoid-man/Obsidian-Notes/blob/da0c222d0562ed5befb13eb2c4dabe0b2dfeaf6f/DBMS%20course/Week%201/assets/Pasted%20image%2020240730130803.png)

Instances keep changing because of the nature of the database. But schemas rarely change unless we need to add a new field. 

Logical Schema is linked to the view (high-level abstraction) and logical schema is also related to the physical schema (the actual bin files or data)

Usually you wouldn't want the logical schema to changes because then the view level and the applications... everything would have to change. 
On the other hand, it may be that the physical schema has to change because of storage or expansion. So it would be better to change the physical schema without changing the logical schema

![Image 5](https://github.com/Schizoid-man/Obsidian-Notes/blob/da0c222d0562ed5befb13eb2c4dabe0b2dfeaf6f/DBMS%20course/Week%201/assets/Pasted%20image%2020240730131432.png)


## Data Models

The meaning of the data stored in our database. It is the real world constraints and relationships which reflect in our database. For eg: Some banks have a minimum bank balance of 5,000 so our database should not allow a balance less than 5000. All these need to factored in when making a bank database.

XML - extensiable markup language

We will most be working on a relational model in this course

![Image 6](https://github.com/Schizoid-man/Obsidian-Notes/blob/da0c222d0562ed5befb13eb2c4dabe0b2dfeaf6f/DBMS%20course/Week%201/assets/Pasted%20image%2020240730141846.png
)

## Data Definition Language (DDL)

Used to define the schema of the database
Eg: `create table instructor(`
	`ID char(5),`
	`name  varchar(20),`
	`dept_name  varchar(20),`
	`salary numeric(8,2)`
`)`


![Image 7](https://github.com/Schizoid-man/Obsidian-Notes/blob/da0c222d0562ed5befb13eb2c4dabe0b2dfeaf6f/DBMS%20course/Week%201/assets/Pasted%20image%2020240730142331.png
)
## Data Manipulation Language (DML)

We'll be using SQL which is a widely used commercial language


