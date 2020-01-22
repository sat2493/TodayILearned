# Structs

TIL an alternative way of declaring struct variables:

```
struct Person
{
    char name[50];
    int citNo;
    float salary;
} person1, person2, p[20];
```

I can access struct variables like the following:

```
person2.salary
```

Examples taken from https://www.programiz.com/c-programming/c-structures
