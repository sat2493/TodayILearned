# Aliasing

TIL that SQL can only extract information from other objects. I wouldn't be able to extract information from subqueries without placing them inside of an alias/variable.

An example of aliasing:

```
SELECT name FROM (SELECT name FROM agentinformation) as a  
```

