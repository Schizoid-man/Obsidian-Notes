> [!WARNING]
> # Attribute

![](assets/Pasted%20image%2020240730204245.png)

## Relation Schema and Instance
![](assets/Pasted%20image%2020240730205559.png)

Basically, if we have Atrributes $(A_1,A_2,A_3...A_n)$ such as `Name`, `USN`, `Aadhar`, `Department`, it has certain domains ($D_1,D_2,D_3... D_N$) such as `String`, `Alphanumeric String`,`12 digit number`,`Alpha String`.
Now a relation is a ==subset== of these domains.
> $r \subset {D_1*D_2*D_3... D_n}$

Since each attribute has an instance ($a_1,a_2,a_3...a_n$) such as `Rahul`,`1MS23CI096`,`126523476891`,`CSE(AIML)`, etc.
So the relational instance for this will be 
> $r \subset a_1,a_2,a_3... a_n$

Also note that because sets have no positional order, and since r is a set, the order of the relations makes no difference.
For eg: instead of having `Name`, `USN`, `Aadhar`, `Department` we can have  `USN`, `Aadhar`, `Name`,`Department`

## Keys
Let K be a subset of R
It is an attribute/a set of attributes that help us identify a row (or tuple) uniquely in a table (or relation)
![](assets/Pasted%20image%2020240730213645.png)

Surrogate keys are basically synthetically produced keys which have no real-world value. For eg: our USNs. USNs do not define us, they dont describe us, nor do they have real-life meaning. They are simply used for identification purposes and to have uniformity. 

If any of the attribute instances are null then it cannot be called a key
__*NO KEY ATTRIBUTE CAN BE A NULLABLE FIELD*__
![](assets/Pasted%20image%2020240804192201.png)
![](assets/Pasted%20image%2020240804192652.png)
If we add 2 other schemas: `Courses` and `Enrolment` then we can see that for the `Courses` schema the primary key is `Course #` and for the `Students` schema the primary key is `Roll #` so now for the `Enrolment` schema we have 2 primary keys: `Roll #` and `Course #`. 
A student may take multiple courses $\implies$ neither `Course#` nor `Roll#` can be used as a primary key. There we consider both of them together as a Primary key. This is called a compound key.

Since `Roll #` belongs to Students schema and `Course #` belongs to Enrolment schema, they are called foreign keys as they both come from 2 different schemas and belong to the Enrolment schema. 
![](assets/Pasted%20image%2020240804195914.png)


## Relational Query Language
![](assets/Pasted%20image%2020240804200638.png)
![](assets/Pasted%20image%2020240804200711.png)
