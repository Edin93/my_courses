#stdarg.h
* strdarg.h is a header in C's standard library that allows functions to accept an indefinite number of arguments.
* It provides facilities for stepping through a list of function arguments of unknown number and type.
* The contents of stdarg.h are typically used in variadic functions.
* It provides the functions and macros to implement the functionnality of variable arguments and follow these steps:
1- define a function with its last parameter as ellipses and the one before it, as int representing the number of arguments.
** int func(int num, ...) { ...
2- create a variable of type va_last in your function.
** va_list myVariable;
3- use int parameter and va_start macro to initialize the va_list variable to an argument list(list of arguments).
** va_start(myVariable, num);
4- use va_arg macro and va_list to access each item in the argument list.
** va_arg(myVariable, int);
5- use the macro va_end to clean up the memory assigned to myVariable.

# Variadic functions
* Variadic functions are function which may take a variable number of arguments and the last parameter is declared as an ellipsis (...). Ex: printf.
* It must have at least one named parameter.

# summery:
* va_list myList; create variable of type va_list in your function.
* va_start(myList, parameters_number);
* va_arg(myList, T); va_arg macro expands to an expression of type T that corresponds to the next parameter from myList.
* va_copy(va_list dest, va_list src); copies src to dest.
* va_end(va_list myList); it performs a cleanup for a myList object initialized by a call to va_start or va_copy.