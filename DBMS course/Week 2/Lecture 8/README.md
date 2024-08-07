# Nested Subqueries
![](../Lecture%207/assets/Pasted%20image%2020240807170159.png)
# Subqueries in the `WHERE` clause
![](../Lecture%207/assets/Pasted%20image%2020240807170549.png)
![](../Lecture%207/assets/Pasted%20image%2020240807170558.png)
- # `SOME` clause
![](../Lecture%207/assets/Pasted%20image%2020240807170739.png)
![](../Lecture%207/assets/Pasted%20image%2020240807170925.png)
`Some` clause basically goes through all the tuples in that attribute and checks if it satisfies the condition for atleast one of them and then it returns a true or false value based on that
If it satisfies the condition for even 1 tuple then it outputs true, else false

- # `All` clause
![](../Lecture%207/assets/Pasted%20image%2020240807171206.png)
![](../Lecture%207/assets/Pasted%20image%2020240807171220.png)
If it satisfies the condition for all the tuples then and only then does it output a true value, else false

- # `Exist` clause
It is used to check if an attribute or a tuple is empty or not
![](../Lecture%207/assets/Pasted%20image%2020240807171545.png)

- # `Not exist` clause
![](../Lecture%207/assets/Pasted%20image%2020240807171644.png)

- # `Unique` keyword
![](../Lecture%207/assets/Pasted%20image%2020240807171812.png)
# Subqueries in `From` clause
![](../Lecture%207/assets/Pasted%20image%2020240807174510.png)
- # `WITH` clause
	![](../Lecture%207/assets/Pasted%20image%2020240807174648.png)

# Subqueries in `Select` clause
![](../Lecture%207/assets/Pasted%20image%2020240807174823.png)
There is a runtime error if the subquery returns more than one value

# Modification of the Database
- ## Deletion
	![](../Lecture%207/assets/Pasted%20image%2020240807175042.png)
	![](../Lecture%207/assets/Pasted%20image%2020240807175149.png)

- ## Insertion
	![](../Lecture%207/assets/Pasted%20image%2020240807175307.png)
	![](../Lecture%207/assets/Pasted%20image%2020240807175414.png)
- ## Updating
	![](../Lecture%207/assets/Pasted%20image%2020240807175637.png)

# `Case` Statement for Conditional Updates
![](../Lecture%207/assets/Pasted%20image%2020240807175826.png)
# Updates with Scalar subqueries
![](../Lecture%207/assets/Pasted%20image%2020240807175921.png)
