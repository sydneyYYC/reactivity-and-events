<script>
  import {recipeName , recipeDescription, inputItem} from '../routes/+page.svelte'
</script>

<div class="bg-amber-700 rounded-lg max-w-[50ch] p-3 m-2 min-h-max flex flex-col items-around">
  <div class="bg-amber-50 p-2 rounded-lg justify-self-start">
  <h4 class="text-3xl font-semibold">{recipeName}</h4>
  <p>{recipeDescription}</p>
  <h6 class="text-xl mt-2">Ingredients</h6>
  <ul class="justify-self-end">
    {#each inputItem as food, i (i)}
    <li>{food}</li>
    {/each}
  </ul>
</div>
</div>
