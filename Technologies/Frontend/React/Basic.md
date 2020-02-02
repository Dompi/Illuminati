# React Basic Concepts

A brief overview about React.

## Components
- Like functions
- Reusable and composable
- Can manage a private state 
- Input: props, state
- Output: UI

## Reactice updates
- When the state of a react component changes, the user interface it represents changes as well
- React will react and automaticly update the part of the browser that need to be updated

## Virtual Views in memory
- Generate HTML using JavaScript
- NO HTML template language
- Tree reconciliation

# Types of React Component

React has two types of components Function and Class components. Both can be state full, can have side effects, or purly presentational.

Capitalization of a component is not optional in react.
 - A component name has to start wth an uppercase letter.
 - HTML elements start with lower case element.

### Function Component
- Much simplier

### Class Component
- More powefull

# Component inputs
- props
  - explicit one
  - imutable
- state
  - internal one
  - use it to auto reflect changes in the browser
  - can be changed

# JSX syntax
Its NOT HTML, but its as close as possible. Its get compiled, for pure javascript functions.
It makes our life easier to code, and read react codes.

# How to display a react component
```
ReactDOM.render(
  <Hello />, 
  document.getElementById('mountNode'),
);
```
- To display a react component in a browser, we need to instruct the ReactDOM libary on how to do that.
- The function designed to do that is ReactDOM.render(), which takes two arguments
  - The first is the component to render (Hello)
  - The second is the DOM element in the browser where we wish the React component to show up. This has to exist in the already rendered HTML before this code.

This is the entry point for React.