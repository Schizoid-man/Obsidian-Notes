
> [!WARNING] CAREFUL!
> YET TO MAKE NOTES FOR THIS LECTURE


# Recap Examples
![](assets/Pasted%20image%2020240806220639.png)
![](assets/Pasted%20image%2020240806220654.png)

# Rename Operation
As discussed previously we can use the `as` keyword to rename an instance or an attribute to suit our needs
![](assets/Pasted%20image%2020240806221220.png)
![](assets/Pasted%20image%2020240806221504.png)

I'll just copy paste chatgpt's answer cos im too sleepy to read through this thing right now:
To solve the given problem using the Cartesian product in relational algebra, we need to find the supervisor of "Bob" and then find the supervisor of the supervisor of "Bob". Here's how we can approach the problem:

    Find the supervisor of "Bob":
        From the given relation emp-super, we can directly see that the supervisor of "Bob" is "Alice".
    Find the supervisor of the supervisor of "Bob":
        We need to find who supervises "Alice". We can look into the emp-super relation again.

Given table:

person  supervisor
Bob     Alice
Mary    Susan
Alice   David
David   Mary

Steps:

    To find the supervisor of "Bob":
        We look at the row where person = 'Bob'. This gives us the supervisor of "Bob", which is "Alice".

    To find the supervisor of "Alice":
        We look at the row where person = 'Alice'. This gives us the supervisor of "Alice", which is "David".

So, the supervisor of "Bob" is "Alice", and the supervisor of "Alice" (which is the supervisor of the supervisor of "Bob") is "David".

Relational Algebra Expression:

    First, select the supervisor of "Bob":
    σperson=′Bob′(emp−super)
    σperson=′Bob′​(emp−super)

    This gives:
    {(′Bob′,′Alice′)}
    {(′Bob′,′Alice′)}

    Then, select the supervisor of "Alice":
    σperson=′Alice′(emp−super)
    σperson=′Alice′​(emp−super)

    This gives:
    {(′Alice′,′David′)}
    {(′Alice′,′David′)}

Alternatively, we can use the Cartesian product to find the supervisor of the supervisor directly:

    Perform a Cartesian product of the emp-super relation with itself:
    R×S={(r1,r2)∣r1∈emp−super and r2∈emp−super}
    R×S={(r1​,r2​)∣r1​∈emp−super and r2​∈emp−super}

    Here, r1r1​ and r2r2​ are tuples from the emp-super relation.

    Select rows where the supervisor from the first relation matches the person from the second relation:
    σR.supervisor=S.person(R×S)
    σR.supervisor=S.person​(R×S)

    Finally, project to find the desired values. For finding the supervisor of the supervisor of "Bob":
    πS.supervisor(σR.person=′Bob′∧R.supervisor=S.person(R×S))
    πS.supervisor​(σR.person=′Bob′∧R.supervisor=S.person​(R×S))

This will give us the result "David", which is the supervisor of "Alice", who is the supervisor of "Bob".

# String Operations
![](assets/Pasted%20image%2020240806221732.png)
![](assets/Pasted%20image%2020240806221942.png)
![](assets/Pasted%20image%2020240806222037.png)
![](assets/Pasted%20image%2020240806222226.png)
![](assets/Pasted%20image%2020240806222542.png)
![](assets/Pasted%20image%2020240806222651.png)
![](assets/Pasted%20image%2020240806223013.png)
![](assets/Pasted%20image%2020240806223120.png)


![](assets/Pasted%20image%2020240806223358.png)
![](assets/Pasted%20image%2020240806223626.png)
![](assets/Pasted%20image%2020240806223708.png)
![](assets/Pasted%20image%2020240806223812.png)
![](assets/Pasted%20image%2020240806224109.png)
![](assets/Pasted%20image%2020240806224150.png)
![](assets/Pasted%20image%2020240806224242.png)
![](assets/Pasted%20image%2020240806224352.png)
