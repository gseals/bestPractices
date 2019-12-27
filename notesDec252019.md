December 25
codecademy:

- if a JSX expression takes up more than one line, then you must wrap the multi-line JSX expression in parentheses
  - ex: const example = (
    <a href="url">
      <h1>
        Click here
      </h1>
    </a>
  );

- a JSX expression must have exactly one outermost element: the first opening tag and the final closing tag of a JSX expression must belong to the same JSX element

- [The Virtual DOM](https://www.codecademy.com/articles/react-virtual-dom) and why React is faster

December 26
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



