# Thinking about DP Optimal Solutions

TIL that a helpful way to think about DP solutions are that they are better alternatives to recursive solutions in terms of runtime. This comes from using more memory, which is a trade off in a way.

In DP, we start from a base case problem and solve with a base case solution. We then cache that solution, and go further and further up the case order. The result is, we never calculate a single solution more than once.
