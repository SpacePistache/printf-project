## _printf Manual Page
![A flow chart showing the step by step process of _printf](_printf.cflowchart.drawio.png)

NAME 
_printf - formats and prints strings and variables to the standard output

SYNOPSIS 
#include "main.h"

##int _printf(const char *format, ...);

DESCRIPTION 
The _printf function formats and prints output to the standard output. It supports a subset of format specifiers, flags, field widths, precision, and length modifiers similar to the standard printf.

Format specifiers available:
%c   Prints a single character.
%s   Prints a string.
%%   Prints a percent sign.
%d   Prints a signed decimal integer.
%i   Prints a signed decimal integer.

Flags, field widths, precision, and length modifiers are not fully implemented. Only the core specifiers listed above are supported.

RETURN VALUE 
The _printf function returns the total number of characters printed, excluding the null byte used to end output to strings. If an error occurs (e.g., if format is NULL), the function returns -1.

EXAMPLES 
Example 1: Printing a simple string _printf("Hello, World!\n"); Output: Hello, World!
Example 2: Printing multiple variables
    _printf("Character: %c, String: %s, Number: %d\n", 'A', "example", 123);
    Output: Character: A, String: example, Number: 123
Example 3: Escaping the percent sign
    _printf("Print 100%% accurate!\n");
    Output: Print 100% accurate!

DATE 
28 NOVEMBER 2024

AUTHORS 
Luke Holley-Boutillier, Ilmi Veliu
