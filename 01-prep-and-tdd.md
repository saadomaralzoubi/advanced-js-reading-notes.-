# Reading notes task 1

## Event Loop :

java script is a single thread languge thats mean it does one thing in the time
some times there is a set time for some functions so browser will stuck till the set time finish .
to solve this problem the event loop came the function with the set time move to webapi and let call stack empty to call the next function ,when the set time finish the function move to the task queue here come the main role for the event loop to see if the call stack is empty it moves the the function from the queue to the call stack.

## call back function :

functions takes parameters as input when we pass a function as a parameter for a nother function its called call back functions.
we use call back to make sure this function will run in a certin time or after a certin function and thats calls asynchronous JavaScript code.

## JS Promises:

Promises are objects return value in future used to handle asynchronous operations in JavaScript. They are easy to manage when dealing with multiple asynchronous operations where callbacks can create callback hell leading to unmanageable code.

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

we use Async await to make our code Asynchronous and both of them are extintions for the promises.
async alow us to use a promis inside the function.
await used to wait the promis, It makes the code wait until the promise returns a result.

## Test-Driven Development:

after we write our code we have to test it, there is two types of tests :
manual: by the user
automated : by testing code

TDD is when you define first the results of your code by the test results after that you start writing your code.
in the outher words your code is drivin by the test .
