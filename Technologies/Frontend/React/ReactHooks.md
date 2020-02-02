# React Hooks

# useState
To use the state object, React has a special function useState().

```
const [counter, setCounter] = useState(initialStateValue);
```
JavaScript function can only return a single value, it will return an array with exactly the two elements here. This is called destructuring feature in JavaScript.

Its returning two items:
- state object (getter)
  - It can be anything string, number, array, anything else
- updater function (setter)


## Example:
How to use, useState function to update a counter on a button on every click. Using an arrov function as an onClick event handler.
```
function Button() {
	const [counter, setCounter] = useState(0);
	return <button onClick={() => setCounter(counter+1)}>{counter}</button>;
}

ReactDOM.render(
  <Button />, 
  document.getElementById('mountNode'),
);
```

