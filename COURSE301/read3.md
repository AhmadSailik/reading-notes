## What does .map() return?
Array
## If I want to loop through an array and display each value in JSX, how do I do that in React?
## Each list item needs a unique ____.
identifies of key
## What is the purpose of a key?
 is a special string attribute you need to include when creating lists of elements.
## What is the spread operator?
The spread operator was added to JavaScript in ES6 (ES2015),It takes in an iterable (e.g an array) and expands it into individual elements.
## List 4 things that the spread operator can do.
- Using Math functions
- Copying an array
- Using an array as arguments
- Adding an item to a list
## Give an example of using the spread operator to combine two arrays.
const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ
## Give an example of using the spread operator to add a new item to an array.
const fewFruit = ['ð','ð','ð']
const fewMoreFruit = ['ð', 'ð', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]
## Give an example of using the spread operator to combine two objects into one.
const objectOne = {hello: "ðĪŠ"}
const objectTwo = {world: "ðŧ"}
const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("ð".repeat(5))}}
objectFour.laugh() // ððððð