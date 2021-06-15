## What is functional programming?
 is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
## What is a pure function and how do we know if something is a pure function?
- It returns the same result if given the same arguments
- It does not cause any observable side effects
## What are the benefits of a pure function?
The code’s definitely easier to test. We don’t need to mock anything
## What is immutability?
In object-oriented and functional programming, an immutable object is an object whose state cannot be modified after it is created. This is in contrast to a mutable object, which can be modified after it is created
## What is Referential transparency?
if a function consistently yields the same result for the same input,
**pure functions + immutable data = referential transparency** 

## What is a module?

## What does the word ‘require’ do?
for use the function in elsewhere in the application
## How do we bring another module into the file the we are working in? 
 require('./count'  )
## What do we have to do to make a module available?
 module.exports=nameOfModule,