# References

TIL that I could pass by reference in C++ to directly modify variables:

```
From: https://www.geeksforgeeks.org/passing-by-pointer-vs-passing-by-reference-in-c/
// C++ program to swap two numbers using 
// pass by reference. 
  
#include <iostream> 
using namespace std; 
void swap(int& x, int& y) 
{ 
    int z = x; 
    x = y; 
    y = z; 
} 
  
int main() 
{ 
    int a = 45, b = 35; 
    cout << "Before Swap\n"; 
    cout << "a = " << a << " b = " << b << "\n"; 
  
    swap(a, b); 
  
    cout << "After Swap with pass by reference\n"; 
    cout << "a = " << a << " b = " << b << "\n"; 
} 
```
