# Input/Output

## printf function
In C, printf is an format function that prints the output on the screen (standard output).  According to different data types in C, the 
parameters in printf are different, see the examples below.  

The the header file ```#include<stdio.h>``` needs to be included before use printf.

Table 1: ```printf``` for basic data types.

| data type        |  format        | example  |
| ------------- |:-------------:| -----:|
| ```int```     | ```%d``` |```int i = 10;``` <br> ```printf("%d", i);``` |
| ```char```    | ```%c```    |  ```char c = "A";``` <br> ```printf("%c", c); ``` |
|```char[]```   |  ```%s```  | ```char str[] = "Informatics-II"``` <br> ```printf("%s", str)``` |




Table 2: The cursor control sequences for the printf command. 

| data type        |  format        |
| ------------- |:-------------:| 
| ```\n``` |    carriage return|
| ```\t``` |       tab      | 
