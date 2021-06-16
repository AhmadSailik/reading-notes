## Understanding the JavaScript Call Stack

## What is a ‘call’?
is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).
## How many ‘calls’ can happen at once?

## What does LIFO mean?
Last In, First Out
## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
## What causes a Stack Overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.

## JavaScript error messages

## What is a ‘refrence error’?
when you try to use a variable that is not yet declared you get this type os errors.
## What is a ‘syntax error’?
this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
## What is a ‘range error’?
var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length
## What is a ‘tyep error’?
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
