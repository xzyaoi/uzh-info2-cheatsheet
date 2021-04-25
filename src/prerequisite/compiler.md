# Compiler


## Recommended Environments

During this course, we will use ```gcc``` as the default compiler for C. If you are using Mac OS or Linux, ```gcc``` should have been installed on your machine. If you are using Windows, you may need an IDE to compile and run your C code. For how to verify and install the environments, please refer to [Installation](./tutorials/installation.html).


##
**<u>Compile a Single Source File</u>**


```gcc example.c -o example.run```

Then we could run the executable file by ```./example.run```.

* The filename is considered as the input file of our compiler. It is passed to the compiler without any parameters.
* The parameter `-o` specifies the output executable file name.
* Some other  useful arguments:
    * `-g` Adds debugging symbols for use with [gdb](https://www.gnu.org/software/gdb/).
    * `-Wall` Enables all compiler warning messages.
    * `-pedantic` Compiler enforces the specified C standard pedantically. 
    * `-std=cxx` Specify a version of C/CPP (by replacing the xx) to compile against.

### Example: 

![helloworldgif](../images/helloworld.gif)
