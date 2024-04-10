Simple Debugger Project

This is a simple debugger project implemented in C programming language. The project consists of two main files:

project.c: This file contains the main implementation of the debugger. It includes functionalities for reading source code from a file, adding directives to the source code, displaying the source code in a terminal using ncurses library, and processing trace variables.

debughdr.h: This header file defines functions for managing trace variables. It includes functions for adding a trace variable, displaying the current value of a trace variable, and updating the value of a trace variable.

How to Use:

Compile the project using a C compiler such as GCC:

(copy to your bash)
gcc project.c -o debugger -lncurses
Run the compiled executable:

(copy to your bash)
./debugger
Use the following commands while running the debugger:

Press 'd' to display the source code.
Press 'w' to move to the previous line.
Press 's' to move to the next line.
Press 'i' to insert a directive into the source code.
Press 'x' to exit the debugger.
Example Usage:

Consider the following sample program, myprog.c:

#include "debughdr.h"

int main() {
    int a, b;
    b = 0;
    a = 1;
    while (b < 10) {
        a = a + b;
        b = b + 1;
    }
    return 0;
}
You can debug this program using the debugger. Add trace variables using the '@var' directive and display them using the '@trace' directive.

Contributing:

Contributions to the project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
