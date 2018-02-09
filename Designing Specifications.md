### Spec Characteristics
* Deterministic and Underdetermined spec
* Declarative and Operational spec
* Stronger and Weaker spec
    * spec strength # the set range of the precondition or postcondition of a module 
    * strong spec # the precondition of a module is stronger or equal than the other one, or the postcondition is 
    weaker or equal than the other one(模块的前置条件太extensive|general or后置条件太narrow|specific)
    * weak spec # the precondition of a module is weaker or equal than the other one, or the postcondition is stronger
     or equal than the other one(模块的前置条件太narrow|specific or后者条件太extensive|general)
 
   
      Ex:
        int binarySearch(int key, int[] arr)
        
        Deterministic spec
           @param key key occurs exactly once in arr
        
        Underdetermined spec
            @param key key occurs in arr(may once, or more than once)
          
          
      Ex:
        Operational spec
        int x = * ptr;// point the value which ptr points to, and assign it to x
    
        Declarative spec
        T *T::operator =(const T &t1);
        //a pointer to T type

### Spec Principles

* Consice # 在满足case computations, method arguments, & return values的情况下，尽可能的减少case computations,
    method arguments, & return values.    
* Precise # The operations or objects of the spec should be deterministic.    
* Sufficient # The spec strength of a module is enough for usage in a particular kind of context. 
* General # The spec should use **abstract types** where possible.
           
      
      Ex: 
        Too Strong spec, should be weak enough.
        
        @param filename a filename to open
        static File open(String filename)
        
     =>
        @param filename read the file stream using a filename from buffer, console, or web server. 
        static File open(String filename)
         
                         
      Ex:
        Template methods & classes in C++
        Interface types in Java
            
        


