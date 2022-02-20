# Reading notes task 1

## Event Loop :

java script is a single thread languge thats mean it does one thing in the time
some times there is a set time for some functions so browser will stuck till the set time finish .
to solve this problem the event loop came the function with the set time move to webapi and let call stack empty to call the next function ,when the set time finish the function move to the task queue here come the main role for the event loop to see if the call stack is empty it moves the the function from the queue to the call stack.

## call back function :

functions takes parameters as input when we pass a function as a parameter for a nother function its called call back functions.
we use call back to make sure this function will run in a certin time .

## JS Promises:

Promises are used to handle asynchronous operations in JavaScript. They are easy to manage when dealing with multiple asynchronous operations where callbacks can create callback hell leading to unmanageable code.

Benefits of Promises :
Improves Code Readability
Better handling of asynchronous operations
Better flow of control definition in asynchronous logic
Better Error Handling

A Promise has four states:
fulfilled: Action related to the promise succeeded
rejected: Action related to the promise failed
pending: Promise is still pending i.e. not fulfilled or rejected yet
settled: Promise has fulfilled or rejected

## JS Async/Await:

Async:
It simply allows us to write promises based code as if it was synchronous and it checks that we are not breaking the execution thread.

Await:
Await function is used to wait for the promise. It could be used within the async block only. It makes the code wait until the promise returns a result.

## Test-Driven Development:

Testing is the process of ensuring a program receives the correct input and generates the correct output and intended side-effects.

Manual Testing:
Manual testing is the process of checking your application or code from the user’s perspective. Opening up the browser or program and navigating around in an attempt to test functionality and find bugs.

Automated Testing:
Automated testing, on the other hand, is writing code that checks to see if other code works. Contrary to manual testing, the specifications remain constant from test to test. The biggest advantage is being able to test many things much faster.
