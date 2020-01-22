# Finding array size

TIL that I could use C's connection to memory to easily find the length of a raw array.

```
From: https://www.tutorialspoint.com/how-do-i-find-the-length-of-an-array-in-c-cplusplus
int arr[5] = {4, 1, 8, 2, 9};
int len = sizeof(arr)/sizeof(arr[0]);
```
