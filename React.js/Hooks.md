# React Hooks

**High Overview**

As everyone knows, React.js all about components, so we need something that can make the component remember the data over time (Through the lifecycle) - and here state concept come.

We can say the state is the 'component memory', and updating the state triggers re-render to display the new state.

---

## useState

in `useState` we can put an initial value (Depends on your need) and it returns 2 things, [value, setValue] and `setValue` is like a function that u can use it to change the `value` - Example:

```jsx
import { useState } from "react";
function ComponentOne() {
    const [welcome, setWelcome] = useState('Good Morning');
    console.log(welcome) // Good Morning
    if(!morning) {
        setWelcome('Good Night')
    	console.log(welcome) // Good Night
    }
}
```

That is easy, But when we need to deal with numbers or Booleans, thing can go different because the values can rely on the previous value.

Example With Booleans:

```jsx
const [isOnline, setIsOnline] = useState(true) // isOnline = true
setIsOnline(previous => !previous) // isOnline = false
```

Example With Numbers:

```jsx
const [increment, setIncrement] = useState(4) // increment = 4
setIncrement(previousNumber => previousNumber + 1) // increment = 5
```



































