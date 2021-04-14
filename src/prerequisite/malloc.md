# Malloc

## Function Signature

`ptr = (cast_type *) malloc (byte_size);`

# Ways of pointer instantiation and declaration

_All examples below construct the same pointer but are syntactically different and some contain superfluous code_.

## Memory allocation

```c
int *pointer = malloc(sizeof int);
```

```c
int *pointer = malloc(sizeof *pointer); // better
```

Note that it is slightly cleaner to write malloc statements by taking the size of the **variable pointed to by using the pointer directly**. If we later rewrite the declaration of ptr the following, then we would only have to rewrite the first part of it:

```c
float *pointer;
/* hundreds of lines of code */
pointer = malloc(sizeof( *pointer));
```

[Source](https://www.cprogramming.com/tutorial/c/lesson6.html)

---

## Type casting

```c
int *pointer = malloc(sizeof *pointer);
```

```c
int *pointer = (int *)malloc(sizeof *pointer);
```

In C, you don't _need_ to cast the return value of malloc. **The pointer to void returned by malloc is automagically converted to the correct type**. However, if you want your code to compile with a C++ compiler, a cast is needed.

[Source](https://stackoverflow.com/a/605856)

---

## Simultaneous declaration and instantiation

```c
int pointer* = malloc(sizeof *pointer);
```

```c
int pointer*;
pointer = malloc(sizeof *pointer); // slightly better?
```

The two statements do exactly the same. Some people suggest that the issue about initializing the result of malloc() is that the allocation may fail.

[Source](https://stackoverflow.com/a/38621955)

---

## Recommendation: Subroutine for "safe-malloc"

The official GNU docs suggest writing a subroutine that calls malloc and reports an error if the value is a null pointer, returning only if the value is nonzero. This function is conventionally called `xmalloc`.

```c
void *xmalloc(size_t size)
{
    void *value = malloc(size);
    if (value == 0)
        fatal("virtual memory exhausted");
    return value;
}
```

[Source](https://www.gnu.org/software/libc/manual/html_node/Malloc-Examples.html)

---

## TL;DR

For this course, it's enough to declare a pointer and assign memory to it like so:

```c
int pointer*;
pointer = malloc(sizeof *pointer);
```

More sources

- [Multiple one line assignments with malloc in c](https://stackoverflow.com/questions/38353667/multiple-one-line-assignments-with-malloc-in-c)
- [How to do one line assignment to malloc() arrays in C?](https://stackoverflow.com/questions/38621377/how-to-do-one-line-assignment-to-malloc-arrays-in-c)
- [Pointers in C 1](https://www.cprogramming.com/tutorial/c/lesson6.html)
- [Pointers in C 2](https://www.programiz.com/c-programming/c-pointers)
- [C Pointers and Memory Allocation](https://www.cs.nmsu.edu/~rth/cs/cs271/notes/Pointers.html)
