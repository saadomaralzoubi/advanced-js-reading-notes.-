## Express REST API

# Questions:

- Name 3 real world use cases where you’d want to change the request with custom middleware ?
  loggin / data api / authorization

- True or false: The route handler is middleware?
  true

- In what ways can a middleware function end the process and send data to the browser?
  when dont put next() in the middlewre.

- At what point in the request lifecycle can you “inject” middleware?
  after sending the rquest and before getting the response .

- What can cause express to error with “Request headers sent twice, cannot start a second response?
  when the middleware stop working .

# Terms :

- middleware:is function gives you access to req and res in the apps request-> response cycle.

- Request Object: Request is used to describe an request to a server.

- Response Object: this is the resopnse coming from the server after the request sent .

- middleware application :software which lies between an operating system and the applications running on it

- Test Driven Diveloment : is when you define first the results of your code by the test results after that you start writing your code.
  in the outher words your code is drivin by the test .

- Behavioural Testing : The testing of external behavior of the program is known as Black Box Testing. It can be applied in software and any program.

# conclusion :

Middleware functions are a really great way to run code on each request, or on each request for a certain route, and to take action on request or response data. Middleware is a crucial piece of any modern web server, and is incredibly useful.
