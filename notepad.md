# notes for building 

## requirements  


1. On the index page, create an array of objects and render it to the page
then add input fields for new values to be added
set up a button that will add the values to the array and update the DOM
use an event modifier (you can use a second button for this example if it makes more sense)

2. Create a component that dispatches an event
your event should render onto the page

3. Create another component that wraps around the component in step 3
use forwarding so that the inner event can be triggered from the page

4. Add a prop (ie: a title) to the outer component and apply that on the page
Create an inline event handler
use this to manipulate css

### Possible builds 

a to-do app

a resource list 

drawing app with tiles - tiling app

notes app

recipe book -- :) lets try it

# steps for input

1. make input fields to take values -- export to component

2. make cards that will hold values

3. push input values into held values

4. render card on page

### building 

- now i have input fields and a place to put those inputs 
- how do i use "bind:value" to take values in svelte?
- i can use https://svelte.dev/repl/116ab042341d48bda2232eae2b6f41a6?version=3.59.2 this resource : 
```
bind:value = {input}

<p> {input}
```