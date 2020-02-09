# Aliasing

TIL that SQL can only extract information from other objects. I wouldn't be able to extract information from subqueries without placing them inside of an alias/variable.

An example of aliasing:

```
From: https://stackoverflow.com/questions/4629979/nested-select-statement-in-sql-server
SELECT name FROM (SELECT name FROM agentinformation) as a  
```

