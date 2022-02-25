# Arrays

First of all, there is a difference between the usage of an array in pseudocode and the usage of an array in C.
When it comes to pseudocode, we use position to describe the elements in an array, and the **position starts at 1**.
While in C programming, we use indices to access the elements in an array, and **the index starts at 0**.
It is important to learn this difference, and you need to be careful about this difference in your practise and your exam.

We take an array of integer as examples. The following also works for arrays of character, double numebr etc.

## An array of integers in Pseudocode
In tasks of exercises and exams, you might see the description like "an array of Integer ```A[]``` with n integers; 
an array of Integer ```A[1..n]```".
 
### scenario 1: an array of integer ```A[]``` with n integers 
The array ```A[]``` is a general way to describe an array, and this array contains n integers. However, we don't know
what these n integer are.
 


### scenario 2: ```A[1..n]```
```A[1..n]``` is equivalent to "an array of integer ```A[]``` with n integers. Remember that in pseudocode, position starts from 1.


For both scenario, the following Pseudocode visits elements of the array ```A[]``` or ```A[1..n]``` from the 
beginning of the array to the end. Note that the array ```A``` has to contain n elements. 

``` c
for(int i = 1; i <= n; i++){
	num = A[i] #access the element at position i.
}
```

## An array of integers in C

In tasks of exercises and exams, you might see the description like "an array of Integer ```A[]``` with \\( n \\) integers".

Let's initialize an array of 4 integers(n = 4) as follows. In C, we have to know the number of elements of an array when
we initialize it.

```c
int A[] = {1, 2, 3, 4}
``` 
 

Remember that the index of an array in C starts from 0. A loop from the first element to the last element is

``` c
for(int i = 0; i <n; i++){
	int num = A[i] // access the element at index i.
}
```
