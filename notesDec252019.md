December 25, 2019
codecademy:

- if a JSX expression takes up more than one line, then you must wrap the multi-line JSX expression in parentheses
  - ex: const example = (
*    <a href="url">
*      <h1>
*        Click here
*      </h1>
*    </a>
  );

- a JSX expression must have exactly one outermost element: the first opening tag and the final closing tag of a JSX expression must belong to the same JSX element

- [The Virtual DOM](https://www.codecademy.com/articles/react-virtual-dom) and why React is faster

December 26, 2019
codecademy:

- in JSX, for tags that are self-closing, such as <br /> and <img />, you must include the closing slash to signify the tag is closed

- writing JS in JSX requires curly brackets:
  - <h1>2 + 3</h1> yields 2 + 3
  - <h1>{2 + 3}</h1> yields 5

- accessing variables within JSX also uses curly brackets.

- an event listener's name should be something like onClick or onMouseOver

- an event's value should be a function

- valid [events](https://reactjs.org/docs/events.html#supported-events) in JSX

- if statements do not work when injected into JSX

- [JSX in depth](https://reactjs.org/docs/jsx-in-depth.html)

- [ternary in JS](https://stackoverflow.com/questions/6259982/how-do-you-use-the-conditional-operator-in-javascript)

- { age > 15 && <h1>Taco</h1> } says that when a number over 15 returns, the <h1> will run

- the 'key' attribute is similar to 'id'
  - A list needs keys if either of the following are true:

  * The list-items have memory from one render to the next. For instance, when a to-do list renders, each item must “remember” whether it was checked off. The items shouldn’t get amnesia when they render.

  * A list’s order might be shuffled. For instance, a list of search results might be shuffled from one render to the next.

  - If neither of these conditions are true, then you don’t have to worry about keys. If you aren’t sure then it never hurts to use them!

- you can use an 'i' in map to create a unique key
  - const example = tests.map((test, i) =>
  <li key={'test_' + i}>{test}</li>
);

- [React](https://reactjs.org/docs/react-api.html#react.createelement) documentation

- you can write React code without JSX. Example:
  - const h1 = <h1>Hello world</h1>; can be written as:
  const h1 = React.createElement(
  "h1",
  null,
  "Hello, world"
);

December 27, 2019
codecademy

- React Components: a component is a reusable piece of code whose job, generally, is to render HTML

- the import React from 'react' line creates a new variable whose name is React and value is a specific imported JavaScript object that contains methods required to run React. The object is the React library

- every component must come from a component class. a component class is like a factory that creates components.

- the body comes within the curly braces that follow the opening curly braces; The body will act as a set of instructions, explaining to your component class how it should build a React component.

- There is only one property that you have to include in your instructions: a render method
  - a render method must contain a return statement. generally, the return statement returns a JSX expression

- class MyComponent extends React.Component
  is a class
  <MyComponent />
  is a component

  Dec 28, 2019
  codecademy

- multi-line JSX expressions should always be wrapped in parenthese

- use curly braces to inject JavaScript into JSX. ex:

  const animal = {
    img: theImage,
    name: theName
  };

  to access these items in JSX, reference the object: {animal.img}, {animal.name}

- render must have a return statement; it can also house other items, like mathematical calculations that need to resolve before the component renders

- conditionals within component class occur inside of render, but before return

- this referes to an instance within the React class

- [understand this in JavaScript](https://dmitripavlutin.com/gentle-explanation-of-this-in-javascript/)

- event listeners: in React, event handlers are defined as methods on a component class

December 28, cont.

- component instances: essentially, nesting one component as the return within another component

- 
