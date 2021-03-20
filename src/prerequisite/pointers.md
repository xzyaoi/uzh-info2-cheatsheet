# Pointers


In C, pointers are widely used to  access variables in memory. Basic concepts of pointers will be explained. 

## Example

```
#include <stdio.h>
 
int main() 
{
  int i = 1;
  int* p_i = &i; // pointer to int i
  //show address of i and the pointer to i
  printf("The address of i is %p \n", &i);
  printf("The address of p_i is %p \n", &p_i);

  // show vaue of i and the pointer to i
  printf("The value of i is %d \n", i);
  printf("The value of p_i is %p \n", p_i);

  //show sizes of i and the pointer to i in memory
  printf("The size of i is %zu bytes \n", sizeof(i));
  printf("The size of p_i is %zu bytes \n", sizeof(p_i));
}
```
Sample output. 
```
The address of i is 0x7ffee52736ac (you should have a different one)
The address of p_i is 0x7ffee52736a0 (you should have a different one) 
The value of i is 1 
The value of p_i is 0x7ffee52736ac (you should have a different one)
The size of i is 4 bytes 
The size of p_i is 8 bytes 
```


Use the ```%p``` formatting specifier to print addresses in hexadecimal. You should see something 
like this: ”0xbfe55918”. The initial characters ”0x” tell you that hexadecimal notation is being used; the remainder 
of the digits give the address itself. Use ```%f``` to print a floating value. Use the sizeof operator to determine the 
memory size allocated for each variable, then use ```%zu``` to print it.


