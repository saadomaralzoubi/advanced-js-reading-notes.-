# Authentication

## Singleton

It is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.

## Singleton with ES6 classes:

The classes should be private constructor , getInstance() methods that returns instance of the class .

We have to export the class name.

## If you were tasked with building a middleware system like Express uses, what approach might I take to construct/operate it?

- I'll create a function with (req,res, next)
- I'll then export it , and require it in the file which contains the express, and use it in the app by using line of code:
  `app.use(middleWare)`

then I can use it in the route handler:
`app.get('/route', (request, response) => {})`

## Term Vocabulary

- Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().
- Dynamic Module Loading:the import(module) expression loads the module and returns a promise that resolves into a module object that contains all its exports. It can be called from any place in the code.
- Singleton pattern : is a software design pattern that restricts the instantiation of a class to one “single” instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.
- CRUD -> REST Method Matches:Create, Read, Update, and Delete.

## Preview:

### Securing Passwords with Bcrypt Hashing Function:

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

#### Hash Collision attack:

Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash. MD5, SHA1, SHA2 are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.

### Bcrypt:

is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.
