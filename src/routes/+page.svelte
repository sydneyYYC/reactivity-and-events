<script>
  import Card from "../lib/Card.svelte";
  import Layout from "./+layout.svelte";
  import {recipeOne, recipeTwo, recipeThree} from '../lib/data.js';
  // import InputCard from "../lib/InputCard.svelte";

  export let recipeName = '';
  export let recipeDescription = '';
  export let inputItem = [];

  // let food = array.push(inputItem);
</script>

<main class="flex flex-col max-h-screen items-center m-4">
<!-- pre made cards -->
<div class="flex max-w-screen block">
  <Card {...recipeOne}/>

  <Card {...recipeTwo}/>

  <Card {...recipeThree}/>

  <!-- <InputCard /> -->
</div>

<!-- new card input  -->
<div class="max-w-screen my-4">

<!-- recipe name input -->
<label for="text-input">Recipe Name</label>: 
<input bind:value={recipeName} placeholder="enter recipe name" class="border-solid border-amber-600 border-2 m-4"/>

<!-- recipe description input -->
<label for="text-input">Recipe Description</label>: 
<input bind:value={recipeDescription} placeholder="enter recipe description" class="border-solid border-amber-600 border-2 m-4 max-w-[50ch]"/>

<!-- recipe ingredient list -->
<label for="text-input">Ingredients</label>: 
<input bind:value={inputItem} placeholder="enter ingredients separately" class="border-solid border-amber-600 border-2 m-4"/>
</div>

<!-- if there is no input the input field card will not show -->
{#if recipeName === ''}
<div> </div>
{:else}
<div id=input-card class="bg-amber-700 rounded-lg max-w-[50ch] p-3 m-2 min-h-max flex flex-col items-around">
  <div class="bg-amber-50 p-2 rounded-lg justify-self-start">
  <h4 class="text-3xl font-semibold">{recipeName}</h4>
  <p>{recipeDescription}</p>
  <h6 class="text-xl mt-2">Ingredients</h6>
  <ul class="justify-self-end">
    {#each inputItem as food}
    <li>{food}</li>
    {/each}
  </ul>
</div>
</div>
{/if}
</main>

