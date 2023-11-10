<script>
export let cardDescription;
export let cardTitle;
export let ingredients = [item];
</script>

<div class="bg-amber-200 rounded-lg min-w-max">
  <h4 class="text-3xl">{cardTitle}</h4>
  <p>{cardDescription}</p>
  <h6 class="text-xl">Ingredients</h6>
  <ul>
    {#each ingredients as item, i (i)}
    <li>{item}</li>
    {/each}
  </ul>
</div>
