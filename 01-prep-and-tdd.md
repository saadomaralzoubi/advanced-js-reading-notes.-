# Reading notes task 1

## Event Loop :

java script is a single thread languge thats mean it does one thing in the time
some times there is a set time for some functions so browser will stuck till the set time finish .
to solve this problem the event loop came the function with the set time move to webapi and let call stack empty to call the next function ,when the set time finish the function move to the task queue here come the main role for the event loop to see if the call stack is empty it moves the the function from the queue to the call stack.

## call back function :

functions takes parameters as input when we pass a function as a parameter for a nother function its called call back functions.
we use call back to make sure this function will run in a certin time .

## JS Promises:
