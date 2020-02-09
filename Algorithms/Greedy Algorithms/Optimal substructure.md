# Optimal Substructure

TIL that some optimization problems can be solved by a greedy algorithm when we our solution has optimal substructure. Often times, this substructure is tested using an if statement. For instance, in the activity selection problem:

```
From: https://en.wikipedia.org/wiki/Activity_selection_problem
Greedy-Iterative-Activity-Selector(A, s, f): 

    Sort A by finish times stored in f
    
    S = {A[1]} 
    k = 1
    
    n = A.length
    
    for i = 2 to n:
       if s[i] ≥ f[k]: 
           S = S U {A[i]}
           k = i
    
    return S
```

The if statement tests whether the current activity start time occurs right after the finish time. This can repetitively be applied where we repeatedly use our greedy comparison to come up with subsolutions. Eventually we get our optimal solution
