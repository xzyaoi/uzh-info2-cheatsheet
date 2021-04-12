# Operators 

Operators are indispensable in programming. We list common and useful operators in C for your study in this course. 


## C Arithmetic Operators
An arithmetic operator performs mathematical operations such as addition, subtraction, multiplication, 
division etc on numerical values (constants and variables).


| Operator        | Meaning of Operator| 
| ------------- |:-------------:| 
| + | addition  | 
| - |subtraction|  
| * | a decimal number| 
| / | division| 
| % | remainder after division (modulo division)| 

### example: Arithmetic Operators
``` c
#include <stdio.h>
int main()
{
    int a = 11;
    int b = 3;
    int c;
    
    c = a+b;
    printf("a+b = %d \n",c);
    
    c = a-b;
    printf("a-b = %d \n",c);
    
    c = a*b;
    printf("a*b = %d \n",c);
    
    c = a/b;
    printf("a/b = %d \n",c);
    
    c = a%b;
    printf("Remainder when a divided by b = %d \n",c);
    
    return 0;
}
```

## C Relational Operators

Relational operators determine one condition is True(1) or False(0), usually used in a loop and if condition.

| Operator        | Meaning of Operator| Example| 
| ------------- |:-------------:|:-------------:|  
|==| equal|```1 == 1```  is evaluated to 0 |
| \> |greater than |int a; int b; a > b |
|\<	|Less than|	```2 < 4``` is evaluated to 1|
|!=| Not equal to|```7 != 2``` is evaluated to 1|
|>=|Greater than or equal to|  ```2 >= 8``` is evaluated to 0|
|<=|	Less than or equal to|	```0 <= -4``` is evaluated to 0||

### example: relational operators
``` c
#include <stdio.h>
int main()
{
    int a = 4, b = 7, c = 11;

    printf("%d == %d is %d \n", a, b, a == b);
    printf("%d == %d is %d \n", a, c, a == c);
    printf("%d > %d is %d \n", a, b, a > b);
    printf("%d > %d is %d \n", a, c, a > c);
    printf("%d < %d is %d \n", a, b, a < b);
    printf("%d < %d is %d \n", a, c, a < c);
    printf("%d != %d is %d \n", a, b, a != b);
    printf("%d != %d is %d \n", a, c, a != c);
    printf("%d >= %d is %d \n", a, b, a >= b);
    printf("%d >= %d is %d \n", a, c, a >= c);
    printf("%d <= %d is %d \n", a, b, a <= b);
    printf("%d <= %d is %d \n", a, c, a <= c);

    return 0;
}
```

