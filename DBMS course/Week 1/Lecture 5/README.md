## Relational Operators:

### Select Operation
If we have a relation (a collection of rows and columns) and we need to select a particular row or column, we use this operation.
It is denoted by $\sigma(r)$ 
We can add conditions $\theta$ (propositional conditions) so that if it satisfies the condition $\theta$ then it will be included in the results otherwise it will not be included.

Eg: ![](assets/Pasted%20image%2020240804220443.png)
![](assets/Pasted%20image%2020240805163003.png)

### Projection Operation
It lets you choose which columns you want and then lets you project it out from the original relation. It is denoted by $\prod(r)$ 
We can mention the columns we want by writing it as a subscript. For eg: if we want the columns A and B we can express it in the following way: $\prod_{A,B}(r)$

Example:
![](assets/Pasted%20image%2020240805163546.png)
Since relations are basically sets, every element has to be distinct and hence it can be done by remove the identical elements (shown in the last step)


### Union of two relations
Denoted by $\cup$
![](assets/Pasted%20image%2020240805164016.png)
### Set difference
Denoted by $\textminus$ 
For eg: r $\textminus$ s will mean ==all the elements in r minus all the elements in s ( in the `r` relation, subtract all the elements which are common between r and s)==

![](assets/Pasted%20image%2020240805164302.png)

### Set Intersection
Denote by $\cap$
![](assets/Pasted%20image%2020240805164740.png)
$r\cap s = r - (r-s)$ hence set intersection is not a fundamental set operation

### Cartesian Product

We can use this to join two tables of equal or unequal sizes
![](assets/Pasted%20image%2020240805165817.png)
If we have two relations which has similar name for its attribute and if we try to join it then we change its name by following this convention:
(*relation from which it is coming from*).(*attribute name*)
![](assets/Pasted%20image%2020240805170144.png)

But now, what if we want to do $r\times r$? then both A and B attributes come from r itself. So we'll get (r.A,r.B)x(r.A,r.B) which makes it confusing while making the database.

Hence we can rename it by use the $\rho$ operator.
If we write $\rho _x (r)$ then we can refer to the r attributes by the letter $x$ 
![](assets/Pasted%20image%2020240805170627.png)


### Composition of relations
![](assets/Pasted%20image%2020240805170822.png)
we can join multiple operations together to get our desired product


# Natural Join Operation
It is denoted by $\bowtie$
Over here, we take the cartesian product of both the relations but only retain the product when the elements of the attributes with common name have the same values. Since the values of these 2 attributes are the same we will only project one of these attributes
![](assets/Pasted%20image%2020240805172218.png)

# Aggregate Operators
- SUM
- AVG
- MAX
- MIN
![](assets/Pasted%20image%2020240805172848.png)
![](assets/Pasted%20image%2020240805172724.png)