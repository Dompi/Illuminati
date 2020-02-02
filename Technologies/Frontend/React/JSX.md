# JSX

JSX is NOT HTML, but its as close as possible. Its get compiled, for pure javascript functions what the browser can understand and execute.
It makes our life easier to code, and read react codes.

## Example
```
function Hello() {
	return <div>Hello React!</div>;
}

ReactDOM.render(
  <Hello />, 
  document.getElementById('mountNode'),
);
```
```
<div>Hello React!</div> -> This is JSX
```
This will not be executed by the browser, it will be executed by the JSX extension and compiled to something else, something the browser can understand.

```
React.createElement("div", null, "Hello React!");
```
So all the JSX elements are compiled to something the browser can understand, even if they embedded.

```
JSX:
ReactDOM.render(
  <Hello />, 
  document.getElementById('mountNode'),
);

Compiled:
ReactDOM.render(
  React.createElement(Hello, null),
  document.getElementById('mountNode')
);
```
## JSX Compilers
 - Babel

# 
JSX supports displaying dinamic expressions if you place them inside in {expression} anywhere inside JSX.

Example: 
- `{Math.random}` -> it will use the random value in every rendering.
- `<button onClick = {logRandom}>Random</button> `
  - logRandom is an event handler function reference.