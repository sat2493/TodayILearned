# NumPy

TIL that NumPy is a fundamental data structure, whose methods are used to store or arrange data.

It is imported through the following:

```
import numpy as np
```

The following generates a graph with titles, a with a legend:

```
company = ['GOOGL', 'AMZN', 'MSFT', 'FB']
revenue = [90, 136, 89, 27]

profit = [40, 2, 34, 12]

plt.xticks(ypos, company)
plt.ylabel("Revenue")
plt.title("US Tech Stocks")
plt.bar(ypos, revenue, label="Revenue")
plt.bar(ypos, profit, label="Profit")
plt.legend()
```

The following generates a horizontal graph:

```
plt.yticks(ypos, company)
plt.xlabel("Revenue")
plt.title("US Tech Stocks")
plt.barh(ypos, revenue, label="Revenue")
plt.barh(ypos, profit, label="Profit")
plt.legend()

ax = plt.gca()
ax.set_xlim([0, 200])
```
