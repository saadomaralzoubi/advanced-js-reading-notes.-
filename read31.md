# Context API

## Context:

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

## When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component.

## Before You Use Context

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

API

React.createContext
Context.Provider
Class.contextType
Context.Consumer
Context.displayName
