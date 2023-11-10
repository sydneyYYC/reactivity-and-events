<script>
  import Card from "../lib/Card.svelte";
  import Layout from "./+layout.svelte";
  import {recipeOne} from '../lib/data.js';
</script>

<main class="flex flex-col max-h-screen items-center m-4">
  <h1 class="my-4 text-2xl font-semibold">Recipe App</h1>

  <Card {...recipeOne}/>

</main>

