<script>
  import Card from "../lib/Card.svelte";
  import {recipeOne} from "../lib/data.js";
  import Layout from "./+layout.svelte";
</script>

<main class="flex flex-col max-h-screen items-center m-4">
  <h1 class="my-4 text-2xl font-semibold">Recipe App</h1>

  <!-- <section class="bg-red-500 min-w-[60%] ">
    <p>Hewwo</p>

  </section> -->
  <Card {...recipeOne}/>

</main>

