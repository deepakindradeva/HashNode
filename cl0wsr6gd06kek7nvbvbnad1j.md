## The Notion of a Good Algorithm

**What is an Algorithm?**

An algorithm is a well-defined computational procedure that takes some value, or a set of values as input and produces some value, or a set of values, as output.

**What is a good algorithm?**

A good algorithm is measured by its running time and space utilization. 
In Laymen's terms:: "*The lesser the better*".

**Can we measure the run time and space utilization of any Algorithm? If Yes, how exactly?**

Yes, we can measure the efficiency of an algorithm by simply determining the Running Time/Memory Space needed by the algorithm to run to completion.

Now, this can be measured in 2 ways-

1. **Time Complexity**:: The time complexity of an algorithm is the amount of time it needs to run to completion.
2. **Space Complexity**:: The space complexity of an algorithm is the amount of space it needs to run to completion

Also, along with this, we should be mindful of the efficiency of algorithms.

1. **Worst-case efficiency**: It is the maximum number of steps that an algorithm has to take for any collection of data values.
2. **Best case efficiency**: It is the minimum number of steps that an algorithm has to take any collection of data values.
3. **Average case efficiency**: It can be defined as the efficiency averaged on all possible inputs.

A graphical representation of the Worst, Best and Average cases of algorithms.
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647617735287/ZXKxNtQbU.png)

**Analysis of Algorithm**

Let's study different methods used in the analysis of algorithms.

**Asymptotic Analysis (Growth of function)**

It simply means a line that continuously approaches a given curve. However, never meets at any finite distance.

For example - 
Let's look at this picture, here X is asymptotic with X+1 as shown in the graph.
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647624968497/OD6ykUtpM.png)

Asymptotic may also be defined as a way to describe the behaviour of functions in the limit or without bounds.

Let f(x) and g(x) be two functions of real numbers.
We say that f and g are asymptotic and write f(x) ≈ g(x) if
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647624907189/R4SxXr9sA.png)

**Asymptotic Notations**
In Asymptotic notations, we ignore the smaller inputs and constants while figuring out complexity.

1. **Big-oh notation**
It provides the upper bound for f(n) and gives the worst-case complexity i.e. the measure of the longest amount of time.
We say that f(n) = O(g(n)), if and only if there are positive constants c and n0 such that
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647628917239/9neys5h7C.png)
If f(n) = O(g(n)), we say that g(n) is an upper bound on f(n).
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647628858148/HftHB97GT.png)
For Example - 
```
F(n) = 3n+2 
as 3n+2≤4n for all n≥2  
=O(n)
F(n) = 3n+3 
as 3n+3≤4n for all n≥3  
=O(n)
```

**NOTE :: K*f(n) is O(f(n))** 
[i.e., constant coefficients can be dropped]
G(n) = 7n4 is O(n4)
That is, if we have a function multiplied by a constant, we can ignore the constant in the big-O.

2. **Big-Omega Notation (Ω)**

It provides the lower bound for f(n) and gives the best-case complexity i.e. the measure of the shortest amount of time.
We can say that f(n) = Ω(g(n)), if and only if there are positive constants c and n0 such that
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647629853782/fm7F-ir5F.png)
If f(n) = Ω(g(n)), we say that g(n) is a lower bound on f(n).
![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1647629721303/Na0tjf-de.png)
