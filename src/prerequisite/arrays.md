# Arrays

First of all, there is a difference between the usage of an array in pseudocode and the usage of an array in C.

When it comes to pseudocode, we use position to describe the elements in an array, and the **position starts at 1**.
While in C programming, we use indices to access the elements in an array, and **the index starts at 0**.
It is important to learn this difference, and you need to be careful about this difference in your practise and your exam.


## An array of integers in Pseudocode

In tasks of exercises and exams, you might see the description like "an array of Integer A[] with n integers".
A loop from the first element to the last element of ```A[]``` is

```
for(int i = 1; i <= n; i++){
	num = A[i] #access the element at position i.
}
```

## An array of integers in C

In tasks of exercises and exams, you might see the description like "an array of Integer ```A[]``` with \\( n \\) integers".

Let's initialize an array of 4 integers(n = 4) as follows.

```c
int A[] = {1, 2, 3, 4}
``` 

with \\(n = 4\\). 

Remember that the index of an array in C starts from \\(0\\). A loop from the first element to the last element is

```c
for(int i = 0; i <n; i++){
	int num = A[i] // access the element at index i.
}
```