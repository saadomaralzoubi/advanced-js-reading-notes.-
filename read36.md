# Application State with Redux

## Terms

### cookies

A block of data that are placed on the user's website or in user's device (third-party cookies) that is used to store data about the user behavior on that website.

### Authorization

The process of giving the user different authorizes (capabilities) after he/she been authenticated.

### Access control

is giving the user different level of access types that will allow the user to interact differently with the website based on user's role or other condition.

### Conditional rendering

rendering the UI based on different conditions, in React, it happens when we use IF component that has a condition if met the children of that component will be rendered.

## Preparation Materials

## Redux

Redux is a predictable state container for JavaScript apps.

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger.

You can use Redux together with React, or with any other view library. It is tiny (2kB, including dependencies), but has a large ecosystem of addons available.

## Redux Toolkit

is the official recommended approach for writing Redux logic. It wraps around the Redux core, and contains packages and functions that we think are essential for building a Redux app. Redux Toolkit builds in our suggested best practices, simplifies most Redux tasks, prevents common mistakes, and makes it easier to write Redux applications.

RTK includes utilities that help simplify many common use cases, including store setup, creating reducers and writing immutable update logic, and even creating entire "slices" of state at once.

Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

npm install @reduxjs/toolkit

Create a React Redux App npx create-react-app my-app --template redux-typescript

Redux Core

npm install redux
