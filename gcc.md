## GCC Flags

	-g
		Generate debugging information in the executable, allowing for debugging with tools like GDB.
	
	-O2
	
		Optimize the compiled code for speed, applying a moderate level of optimization.
		
	-std=c++11, -std=c++14, -std=c++17, -std=c++20
		
		Specify the C++ language standard 
	
	-I<path>
	
		Add the specified directory to the list of directories to be searched for header files during compilation.

	-L<path>
		
		Add the specified directory to the list of directories to be searched for library files during linking.

	-l<library> 
		
		Link against the specified library during the linking phase.

	-pthread
	
		Enable support for multithreading with the POSIX threads library.

	-fPIC
		
		Generate position-independent code, which is required for creating shared libraries.

	-shared
	
		Generate a shared library rather than an executable.
	
	-pedantic-errors 

		strict conformance to C/C++ standards

	-Wall -Weffc++ -Wextra 

		adherence to best practices in C++

	-Wconversion -Wsign-conversion

		identify potential precision loss or unintended behavior when converting between different types, including conversions between signed and unsigned types

	-Werror

		Treat all warnings emitted by the compiler as errors
		
## GCC Debug

g++ -g -o hello hello.cpp
gdb hello
	
+ **break or b**: Set breakpoints at specific lines or functions where you want the program to pause. Ex: break main
+ **run or r**: Start executing the program until it reaches a breakpoint or completes.
+ **next or n**: Execute the next line of code, stepping over function calls.
+ **step or s**: Execute the next line of code, stepping into function calls.
+ **print or p**: Print the value of a variable or expression. Ex: print myvar
+ **backtrace or bt**: Display the current call stack.
+ **continue or c**: Continue program execution until the next breakpoint or until the program finishes.
+ **quit or q**: Exit GDB.

	
	
