<script>
export let cardDescription;
export let cardTitle;
export let ingredients = [item];
</script>

<div class="bg-amber-700 rounded-lg max-w-[50ch] p-3 m-2 min-h-max flex flex-col items-around">
  <div class="bg-amber-50 p-2 rounded-lg justify-self-start">
  <h4 class="text-3xl font-semibold">{cardTitle}</h4>
  <p>{cardDescription}</p>
  <h6 class="text-xl mt-2">Ingredients</h6>
  <ul class="justify-self-end">
    {#each ingredients as item, i (i)}
    <li>{item}</li>
    {/each}
  </ul>
</div>
</div>
