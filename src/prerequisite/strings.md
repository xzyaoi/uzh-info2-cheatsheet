# Strings

In C, there is no string data type. In practise, a string is an array of characters(char). 

## Termination Character

A string is an array of characters with a terminating character ```'\0'```.

## Useful Functions

Assume that we have a string ```char str[]```. The following function ```int len(char str[])```calculates the length of a string. 
```
int len(char str[]) {
    int i;
    while(str[i] != '\0') {
        i++;
    }
    return i;
}
```