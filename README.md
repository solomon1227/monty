# 0x19. C - Stacks, Queues - LIFO, FIFO
```C``` ```Group project``` ```Algorithm``` ```Data structure```

**Group project on C programming at ALX software engineering**
By
- **Solomon Ferede - solomonf1227@gmail.com** and
- **Mesfin Fikrea - https://github.com/mesfik**
## Requirements
### General
- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 20.04 LTS using gcc, using -the options -Wall -Werror -Wextra -pedantic -std=c89
- All your files should end with a new line
- A README.md file, at the root of the folder of the project is mandatory
- Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
- You allowed to use a maximum of one global variable
- No more than 5 functions per file
- You are allowed to use the C standard library
- The prototypes of all your functions should be included in your header file called monty.h
- Don’t forget to push your header file
- All your header files should be include guarded
- You are expected to do the tasks in the order shown in the project


## Compilation & Output
```$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty```
- Any output must be printed on ```stdout```
- Any error message must be printed on ```stderr```

## The monty program

- Usage: ```monty file```
	- where ```file``` is the path to the file containing Monty byte code
* If the user does not give any file or more than one argument to your program, print the error message ```USAGE: monty file```, followed by a new line, and exit with the status ```EXIT_FAILURE```
* If, for any reason, it’s not possible to open the ```file```, print the error message ```Error: Can't open file <file>```, followed by a new line, and ```exit``` with the status ```EXIT_FAILURE```
	- where <file> is the name of the file
- If the file contains an invalid instruction, print the error message ```L<line_number>: unknown instruction <opcode>```, followed by a new line, and exit with the status ```EXIT_FAILURE```
	- where L is the line number where the instruction appears.
Line numbers always start at 1
- The monty program runs the bytecodes line by line and stop if either:
	- it executed properly every line of the file
	- it finds an error in the file
	- an error occured
- If you can’t malloc anymore, print the error message ```Error: malloc failed```, followed by a new line, and exit with status ```EXIT_FAILURE```.
- You have to use ```malloc`` and ```free``` and are not allowed to use any other function from man malloc (realloc, calloc, …)

## Authors
- **Solomon Ferede - solomonf1227@gmail.com** and
- **Mesfin Fikrea - https://github.com/mesfik**

## Files included in the repo
- ```README.md``` - Description about the project.
- ```Monty.h``` - Header file containing the prototype of the function and structure defination.
- ```monty.c``` - main function  - reading file from command line
- ```error_handler.c``` - handle the error and rint it to stderr
- ```functions_on_stack.c``` - File containing functions performed on stuck elemets
- ```operation_on_stuck_element.c``` - A file containg functions performing swap element, addation,.... on elements of stuck
- ```parse.c```- File containg of functions used to open, read and interpret the opcode
- ```stack_operation.c``` - File containg of functions used to push, pall operation
- ```string_handle.c``` - handle the strings in stack
