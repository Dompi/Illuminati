# Functional Component

Simple function component, named Hello which is returns a div.
### Code:
```
function Hello() {
	return <div>Hello React!</div>;
}
```
- This component has no input.
- This is a pure component because has no state.

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

# Usefull styling

```
function Button() {
	const [counter, setCounter] = useState(0);
	return ( 
    <button onClick={() => setCounter(counter+1)}>
      {counter}
    </button>
    );
}

ReactDOM.render(
  <Button />, 
  document.getElementById('mountNode'),
);
```
- In return use () because you not return an object you return a function call, the ``React.createElement(Button, null)`` function call in the ReactDOM.render() function. 
- 

