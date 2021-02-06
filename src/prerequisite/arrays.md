# Arrays

## An array of integers

In tasks of exercises and exams, you might see the description like "an array of Integer ```A[]``` with \\( n \\) integers".

In C programming, we declare an array of integer as follows.

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