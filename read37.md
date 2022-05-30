# Combined Reducers

## Terms

### Immutable state

state can not be changed.

### Time travel in redux

The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

### Action creator

is an object that has type and payload property.

###Reducer
A pure function that takes in an action and state, return new state based on the action.

### Dispatch

A function of the Redux store. to dispatch an action to components. This is the only way to trigger a state change. With React Redux, your components never access the store directly, you need to dispatch actions in component with type and payload to change the state.

## Preparation Materials

### Combined Reducers

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key.<br>

The most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same `(state, action)` signature, and each responsible for managing all updates to that specific slice of state.<br>
Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.<br>

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by `combineReducers()` namespaces the states of each reducer under their keys as passed to `combineReducers()`. <br>

Any reducer passed to combineReducers must satisfy these rules:

- For any action that is not recognized, it must return the state given to it as the first argument.

- It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.

- If the state given to it is undefined, it must return the initial state for this specific reducer. According to the previous rule, the initial state must not be undefined either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being undefined.
