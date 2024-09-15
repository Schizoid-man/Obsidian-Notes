<<<<<<< HEAD
![[assets/Pasted image 20240812190932.png]]
# Accessing SQL from a Programming Language
![[assets/Pasted image 20240812191028.png]]
Few important APIs for SQL integration:
- JDBC (for java)
	![[assets/Pasted image 20240812191126.png]]
- OBDC
	![[assets/Pasted image 20240812191213.png]]

![[assets/Pasted image 20240915171857.png]]

![[assets/Pasted image 20240915172130.png]]

![[assets/Pasted image 20240915172541.png]]

![[assets/Pasted image 20240915172652.png]]

We also have functions in SQL but we don't use them that often
![[assets/Pasted image 20240915172846.png]]
![[assets/Pasted image 20240915172938.png]]
We mostly dont use language constructs in SQL but we may use the for loop sometimes to repeat a certain operation in the table
![[assets/Pasted image 20240915173056.png]]
most of these arent useful to us as SQL is mostly a declarative language and hence doesnt require procedural arguments to be used often.

# Triggers
Basically a flag
![[assets/Pasted image 20240915173506.png]]
![[assets/Pasted image 20240915173619.png]]

For a trigger to work we need an old row and a new row. The trigger checks the value of the old row and then 'references' the value of the new row and then makes changes to that row.

So the trigger looks at the old row and makes a change in the new row

Example:
![[assets/Pasted image 20240915173826.png]]
![[assets/Pasted image 20240915174009.png]]


=======
# Accessing SQL from a programming language
![](assets/Pasted%20image%2020240818185247.png)

![](assets/Pasted%20image%2020240818185329.png)
Examples:
- JDBC
- ODBC
- etc...

![](assets/Pasted%20image%2020240818185418.png)
Here we're embedding the SQL within the C program

# Embedded SQL
![](assets/Pasted%20image%2020240818185513.png)

![](assets/Pasted%20image%2020240818185619.png)

![](assets/Pasted%20image%2020240818185648.png)

![](assets/Pasted%20image%2020240818185711.png)
![](assets/Pasted%20image%2020240818194951.png)

![](assets/Pasted%20image%2020240818195217.png)

![](assets/Pasted%20image%2020240818195328.png)

There are many other native procedural features in SQL also which I am going to skip since it is rarely used 

# Trigger
![](assets/Pasted%20image%2020240818195845.png)
![](assets/Pasted%20image%2020240818200627.png)
![](assets/Pasted%20image%2020240818200945.png)

![](assets/Pasted%20image%2020240818201047.png)
![](assets/Pasted%20image%2020240818201129.png)
>>>>>>> origin/main

