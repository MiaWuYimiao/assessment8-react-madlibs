### Conceptual Exercise

Answer the following questions below:

- What is React? When and why would you use it?
  > React is a popular, powerful front-end framework.
  - React make it easy to make reusable "view components"
    - These "encapsulate" logic and HTML into a class
  - Often make it easier to build modular application

- What is Babel?
  > Babel is a transpiler that turns input code into "pure" JavaScript.  
  Babel can transform the latest JavaScript features, which are not understandable to every browser, into a backward compatible version of JavaScript in current and older browsers of environments.

- What is JSX?
  > JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.

- How is a Component created in React?
  > Component can be created as a function component or class component in React.

- What are some difference between state and props?
  - Props are used to pass data from a parent component to child component, while state is used to manage data within a component.
  - Props are immutable and cannot be changed within a component, while state is mutable and can be updated using the setState function.

- What does "downward data flow" refer to in React?
  > Downward data flow is the idea that parent components pass data down to their children via props. In order to make data go the other way, we have to pass a function down from the parent that the chil can then call with some information.
    - A parent component defines a function
    - The function is passed as a prop to a child component
    - The child component invokes the prop
    - The parent function is called, usually setting new state
    - The parent component is re-rendered along with its children

- What is a controlled component?
  > In React, a controlled component is a component that is controlled by React state. 

- What is an uncontrolled component?
  > If React is not in control of the form state, this is called an uncontrolled component.

- What is the purpose of the `key` prop when rendering a list of components?
  > **key** is a special string attr to include when creating lists of elements.
   - Keys help React identify which items are changed/added/removed.
   - Keys should be given to repeated elems to provide a stable identity.

- Why is using an array index a poor choice for a `key` prop when rendering a list of components?
  > Because item order may change or items can be deleted. This can cause performance problems or bugs with component state.

- Describe useEffect.  What use cases is it used for in React components?
  > useEffect is a built in hook in React for "side effects". It can be used to fetch data, start a timer and manually changing the DOM.  
  It's very common that when a component renders, we can use useEffect  to fetch data from an external data source or API. Or it can be used to fetch data not after the first render, but after a later state change. useEffect can also be used to clear intervals or timeouts, remove an event listener, unsubscribing and disconnect from a socket.

- What does useRef do?  Does a change to a ref value cause a rerender of a component?
  > useRef is another built-in hook in React. It returns a mutable object with a key of current, whose value is equal to the initial value passes into the hook. The object persists across renders. Mutating the object does not trigger a re-render.

- When would you use a ref? When wouldn't you use one?
  > When I need to access an underlying DOM element, setting up or clearing timers.  
    useRef should not be used to access the DOM and make changes(toggle classes, set text, etc).

- What is a custom hook in React? When would you want to write one?
  > Custom Hooks
    - A JavaScript function that typically uses built in hooks
    - The function name of a custom hook should start with use (useToggleState)
    - Custom hooks can be reusable across different components
  > When to write one?
    - Same business logic inside of multiple components
    - Business logic cluttering up a single component
    - Refactor code

