<script>
export let cardDescription = 'this is a recipe for a card that is good and tasty mmm yum yum yum yum';
export let cardTitle = 'chicken cream';
export let ingredients = [
  {item: 'chicken'},
  {item:'cream'}
   ]; 
</script>

<div class="bg-amber-200 rounded-lg min-w-max">
  <h4 class="text-3xl">{cardTitle}</h4>
  <h6 class="text-xl">Ingredients</h6>
  <ul>
    {#each ingredients as {item}}
    <li>{item}</li>
    {/each}
  </ul>
  <p>{cardDescription}</p>
</div>
