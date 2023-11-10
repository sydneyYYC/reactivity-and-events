<script>
export let cardDescription;
export let cardTitle;
export let ingredients = [item]; 
</script>

<div>
  <h4 class="text-3xl">{cardTitle}</h4>
  <h6 class="text-xl">Ingredients</h6>
  <ul>
    {#each ingredients as {item}}
    <li>{item}</li>
    {/each}
  </ul>
  <p>{cardDescription}</p>
</div>
