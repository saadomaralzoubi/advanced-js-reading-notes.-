# Reading: useState() Hook

Hooks apply the React philosophy inside a component, rather than just between the components. That’s why I feel that Hooks are a natural fit for the React component model. Unlike patterns like render props or higher-order components, Hooks don’t introduce unnecessary nesting into your component tree.

## Do Hooks Make React Bloated?

If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props. The Hooks proposal doesn’t include any breaking changes. Your existing code would keep on working even if you adopted Hooks in the newly written components.

## What Are Hooks, Exactly?

To understand Hooks, we need to take a step back and think about code reuse. Today, there are a lot of ways to reuse logic in React apps. We can write simple functions and call them to calculate something. We can also write components (which themselves could be functions or classes). Components are more powerful, but they have to render some UI. This makes them inconvenient for sharing non-visual logic. This is how we end up with complex patterns like render props and higher-order components. Wouldn’t React be simpler if there was just one common way to reuse code instead of so many?

Functions seem to be a perfect mechanism for code reuse. Moving logic between functions takes the least amount of effort. However, functions can’t have local React state inside them. You can’t extract behavior like “watch window size and update the state” or “animate a value over time” from a class component without restructuring your code or introducing an abstraction like Observables. Both approaches hurt the simplicity that we like about React.

Hooks solve exactly that problem. Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.

## hooks with Classes

Custom Hooks are, in our opinion, the most appealing part of the Hooks proposal. But in order for custom Hooks to work, React needs to provide functions with a way to declare state and side effects. And that’s exactly what built-in Hooks like useState and useEffect let us do. You can learn about them in the documentation.

It turns out that these built-in Hooks aren’t only useful for creating custom Hooks. They are also sufficient for defining components in general, as they provide us with all the necessary features like state. This is why we’d like Hooks to become the primary way to define React components in the future.

We have no plans to deprecate classes. At Facebook we have tens of thousands of class components and, like you, we have no intention of rewriting them. But if the React community embraces Hooks, it doesn’t make sense to have two different recommended ways to write components. Hooks can cover all use cases for classes while providing more flexibility in extracting, testing, and reusing code. This is why Hooks represent our vision for the future of React.
