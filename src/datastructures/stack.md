# Stack

In slides, you can see the following pseudocode:

```
Algo: push(x)

S[t] = x;

t = t+1;
```
It is assumed that the stack S is a global variable, so S is not a paramater of push function. 

In C, Algo: push(x) is implemented as follows.
```
#include <stdio.h>
 
/* global variable declaration */
int S[10];
int t = 0;

void push(int x){
    S[t] = x;
    t = t + 1;
    return;
}
 
int main () {
    /* local variable*/
    int x = 1;
    push(x);
    return 0;
}

```
When using global variables, you need to be careful about which variables are called.
