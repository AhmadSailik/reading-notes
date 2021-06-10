## What is a ‘Controlled Component’?
- combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input.
## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
 because you need to write an event handler for every way your data can change and pipe all of the input state through a React component.
## How do we target what the user is entering if we have an event handler on an input field?
- use uncontrolled components