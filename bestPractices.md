## Notes

* Any time you copy-paste code, you should be looking for a way to simplify or make a variable.

* function names should be verbs and descriptive of what task they perform.

* name things explicitly

* don't ever make buttons that just say "Next"
  * be descriptive so the user knows what will happen when the button is pressed

* seek feedback from people in target group, but not involed in the group or project

* use Target in the console to find the id

* DRY coding - don't repeat yourself

* make your functions as dynamic as possible by omitting special names within the function that relate to the immediate data you are using

* it's hard to overwrite bootstrap, but you can hard code bootstrap into your code and modify it: [bootstrap source code](https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.css);

* \ means "escaping." This symbol signals that the next character should not be considered code and that it should be treated as a string character. Example: 'you can\'t drive' If the escape symbol were left out, the string would end at "can."

* everything is an object in JS.

* comment regularly to clarify the functions in your code. Good commenting communicates the intent of your code - both for others and your future self.

* array methods: .shift() removes and holds first element from array; .unshift() adds to the first position in an array; .pop() removes and holds last element from array; .push() adds an item to the end of an array

* concise body arrow functions:
  * zero parameters: const functionName = () => {};
  * one parameter: const functionName = paramOne => {};
  * two or more parameters: const functionName = (paramOne, paramTwo) => {};

* don't define variables in the global scope; if a variable does not need to exist outside the block, it shouldn't

* always increment the loop; otherwise, you will create an infinite loop

* when running modules without webpack, always remember the type="module" in the script tag at the bottom of the HTML to enable the import/export

* e.preventDefault() in every click function

* $(e.target) is our magic bullet

* apply click event to body

* init function is an organizational piece that gathers everything that needs to run on page load

* with an input and label, id & for have to match

* with ES6 modules, type="module" must be present

* technical debt: you want to find the fastest solution to deployment; determine when is best for you to build a bigger project