# Effective Objective C

1. Objc uses a message structure rather than function calling
     message structure, the runtime decides which code get executed
    * function calling, thie compiler decides which code will be executed
    * polymorphism in function calling, runtime lookup in virtual table
    * messaging, dynamic binding
        >  You declare a variable that is to hold a reference to an object

2. The memory for Objective-C objects is always allocated in heap space and nevar on the stack.
   * heap-allocated 
   * stack-allocated
   * c struture used where the overhead of using Objc objects could affect performance
   * memory-management architecture,  reference counting

3. @class, farward declaring a class
   > chicken-and-egg situation
    