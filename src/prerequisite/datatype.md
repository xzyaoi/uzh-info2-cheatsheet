# C basic data types

In the exercises, you will frequently see the following C data types.


| Type        | Explanation          | example  |
| ------------- |:-------------:| -----:|
| int      | an integer with range (from −2,147,483,648 to +2,147,483,647) | int a = 10; |
| char      | a character      |   char c = 'a'; |
| float | a decimal number      |   float grade = 5.50; |
| Double | a decimal numer      |   double pi = 3.1415926; |

In C, the data type of a variable should be defined before used. Although there are
some way to convert one data type to another, type casting is not suggested. 

## Counterexample
(1) mixed data type
``` c
int a = 2;
float b = 2.0;
int c = a + b;
float d = a + b; 
```
Since a and b have different data types, C complier will do data type casting for c and d.
This is not suggested.

Solution:
Make a and b the same data type.
```c
float a = 2.0;
float b = 2.0;
folat c = a + b; 
```

```c
int a = 2;
int b = 2;
int c = a + b; 
```



