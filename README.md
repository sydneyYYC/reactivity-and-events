# CPNT 262 Assignment 5
## Reactivity and Events
## Sydney Bruce
## [livepage]

#### Bugs and Research 

- having an issues importing data into my card from my separate file . i want to do it this way so i can push data into the card data fields without messing with my card too much . 

- fixed. used this syntax with i as iterator to cycle through ingredients list  https://svelte.dev/repl/a3f0f86ca2014efeb3db9ea3fbd5c21b?version=3.38.3 . thanks svelte docs :) 

- input fields https://svelte.dev/examples/text-inputs 
- now i have input fields and a place to put those inputs 
- how do i use "bind:value" to take values in svelte?
search terms [bind: value svelte]

- i can use https://svelte.dev/repl/116ab042341d48bda2232eae2b6f41a6?version=3.59.2 this resource : 
```
bind:value = {input}

<p> {input}
```

- this works BUT i cant add items as array, items are being added as individual strings - which is not good 
- can i add items and divide ingredients by ' ' ? 
search terms [array.pop], [array svelte], [working with arrays svelte]

- ok i need to add a button to submit my values into a separate card. 
- ok NOW using this https://svelte.dev/repl/8eb540552faa4651a398b182fa5cdd48?version=4.2.3 i have added a click handler to my button to run a function. 

search terms [click handler svelte]

- now i need to write a function that will insert my input values into a new card and push it to the first array. 

- ok so that didnt work. BUG it broke it . if i change my rendering of cards into an each loop from an array and push my new values to that array with .push can i render a new array ? 

- pushing to a new array has proven not successful 

- https://svelte.dev/repl/118b7d4540c64f8491d10a24e68948d7?version=3.12.1 DOM elements in Svelte
- by using the child/container and append child syntax i can push elements to the page but i am getting "[object Object]", slightly closer but i want to target the added input values. hmmmmmmmmmmmmmmm

- i ended up erasing my onclick from my button and using a on:submit through my form. 

