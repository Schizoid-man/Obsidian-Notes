# Joined relations
![](assets/Pasted%20image%2020240807182240.png)

## Types of Join between relations
![](assets/Pasted%20image%2020240807180309.png)

# Examples
![](assets/Pasted%20image%2020240807180938.png)

# Inner Join
![](assets/Pasted%20image%2020240807181313.png)

# Outer Join
![](assets/Pasted%20image%2020240807181959.png)
- Left outer join
	![](assets/Pasted%20image%2020240807182014.png)
- Right outer join
	![](assets/Pasted%20image%2020240807182046.png)
	

# Full Outer Join
![](assets/Pasted%20image%2020240807182336.png)


| Type                | Definition                                                                                                                                                                            | Syntax                                                                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Cross Join**      | Basically its just the cartesian product of the rows from the table                                                                                                                   | Explicit: select * from employee cross join department                                                                                                  |
|                     |                                                                                                                                                                                       | Implicit: select * from employee, department                                                                                                            |
| **Inner Join**      | We take the cross product and then only retain the rows which have matching tuples and discard the rest                                                                               | (relation name) inner join (another relation name)<br><br>if `natural` is used then the 2nd set of common attributes from the 2nd relation is discarded |
| **Outer Join**      | We take the cross product and we dont delete any rows and the values which are not known are assigned the `null` value. Can be of two types: _Left outer join_ and _Right outer join_ |                                                                                                                                                         |
| _Left Outer Join_   | We take the relation given on our left as the dominant relation and show all the tuples in that but we discard the unique rows from the relation given on the right                   | course natural left outer join prereq                                                                                                                   |
| _Right Outer Join_  | We take the relation given on our right as the dominant relation and show all the tuples in that but we discard the unique rows from the relation given on the left                   | course natural right outer join prereq                                                                                                                  |
| **Full Outer Join** | It takes the cross product of all the rows and we dont delete any values. If a certain value is unknown then it is assigned the `null` value.                                         | course natural full outer join prereq                                                                                                                   |
# `On` keyword

We can use the on keyword to mention which conditions and attributes to use when joining two relations
![](assets/Pasted%20image%2020240807182604.png)

# `Using` keyword

We can use that to mention which attribute to use and compare while joining two relations
![](assets/Pasted%20image%2020240807182833.png)

---

# Views
![](assets/Pasted%20image%2020240807183226.png)
![](assets/Pasted%20image%2020240807183348.png)
![](assets/Pasted%20image%2020240807183511.png)
![](assets/Pasted%20image%2020240807183551.png)
![](assets/Pasted%20image%2020240807183622.png)
![](assets/Pasted%20image%2020240807183706.png)
![](assets/Pasted%20image%2020240807183727.png)
As long as the view definitions are not recursive, this loop will
terminate
# Recursive View
![](assets/Pasted%20image%2020240807183840.png)
- Seed statement (non-recursive)
- Recursive statement
- Connection Operator (UNION ALL)
- Terminal condition
![](assets/Pasted%20image%2020240807184101.png)
![](assets/Pasted%20image%2020240807184428.png)
![](assets/Pasted%20image%2020240807184459.png)
![](assets/Pasted%20image%2020240807184609.png)
![](assets/Pasted%20image%2020240807184620.png)

# Updating a View
![](assets/Pasted%20image%2020240807184735.png)
![](assets/Pasted%20image%2020240807184747.png)
![](assets/Pasted%20image%2020240807184810.png)
![](assets/Pasted%20image%2020240807184831.png)
![](assets/Pasted%20image%2020240807184923.png)

# Transactions
![](assets/Pasted%20image%2020240807185018.png)


