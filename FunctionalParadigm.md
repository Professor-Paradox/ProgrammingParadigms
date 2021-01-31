lambda calculus
pure functions:same output with same input
data is immutable can't change present data but can copy to new one and modify
recursion

functions are first class and are higher order
can be used as variable and hold data,pass as arguments to other functions,here the address of the function is passed.  
This implements in having nested functions. 


referential transparency since every time a function gives the same output we can easily replace the function in our code to the result it will give.  
pure functions+immutable=referential transparency
Ex: square(2) always gives 4 so in our code we can remove square(2) and give 4 directly.  

