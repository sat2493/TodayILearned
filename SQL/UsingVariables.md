# Using Variables

TIL that I can actually use variable names in my queries:

```
SELECT COUNT(CITY) - COUNT(DISTINCT CITY) AS N FROM STATION;
```
