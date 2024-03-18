**Data** : Any information that can be moved, processed, or stored by a computer.  
**Object** : A region of storage (usually memory) that can store a value. In C++ objects can be unnamed or named.  
**Variable** : An object with a name. At runtime, the variable is instantiated i.e. an object is created and assigned a memory.  
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

