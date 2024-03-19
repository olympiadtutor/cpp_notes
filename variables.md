**Data** : Any information that can be moved, processed, or stored by a computer.  
**Object** : A region of storage (usually memory) that can store a value. In C++ objects can be unnamed or named.  
**Variable** : An object with a name. At runtime, the variable is instantiated i.e. an object is created and assigned a memory.
**Literal** : A fixed value that is inserted directly into the source code. Literal’s value is placed directly in the executable, and the executable itself can’t be changed after it is created while variable’s value is placed in memory, and the value of memory can be changed while the executable is running.
```cpp
#include <iostream>
int main(){
    std::cout << 5 << '\n'; // print the value of a literal
    int x { 5 };
    std::cout << x << '\n'; // print the value of a variable
    return 0;
}
```
**Data Type** : Tells the compiler what type of value the variable will store. The type must be known at compile-time.  
**Initialization** : Assigns the initial value for an object when its created. Assignment gives value at some point after variable is created. 
- **Copy Initialization** :
  ```cpp
  int width = 5
  ```
- **Direct Initialization** :
  ```cpp
  int width( 5 )
  ```
- **List Initialization** :
  ```cpp
  int width { 5 }
  int height = { 6 }
  int depth {} // value initialized to zero.
  int width { 4.5 }; // error: fractional value can't fit into int
  ```
  Copy and direct initialization simply drop the fractional part, resulting in the initialization of value 4 into variable width. Compiler may optionally warn about this. However, with list initialization, compiler is required to generate error.

**Operator** : An operation is a process involving zero or more input values (called operands) that produces a new value (called an output value). The specific operation to be performed is denoted by a symbol called an operator.
| Type | Description | Example|
|------|--------------|-------|
|Unary  | One operand   | "-" operator which flips sign of operand Ex: -5         |
|Binary | Two operand   | "+" operator which adds Ex: x + y                       |  
|Ternary| Three Operand | "?" conditional operator Ex: var = (y < 10) ? 30 : 40   |
|Nullary| Zero Operand  | throw operator                                          |


