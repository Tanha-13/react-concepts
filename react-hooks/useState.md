## Definition
useState is function that adds and manages state to functional components in React. It provides a way to declare and manage state variables directly within a function component. One use of useState() can only be used to declare one state variable.

---

## Importing `useState` hook
to import `useState` hook from react:
```
    import {useState} from "react";
```
## Structure
```
    Syntax:
    const [state, setState] = useState(initialState);

    Example:
    const [age,setAge] = useState(14);
```
**Call `useState` at the top level of your component to declare a state variable.**
### initialState
The argument passed to useState is the initial value that is set to the `state` variable. It can be a value of any type. This argument is ignored after initial render.

### Returns
useState returns an array with two values: *state(the current state)* and *set function to update the state  to a different value and trigger a re-render.*
- During the initial rendering, the returned status(state) is the same value as the first argument passed in (initialState).
- `setState` function receives a new state value and queues a re-render of the component.