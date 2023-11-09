<script>
export const navItems = [
  {name:'recipies', href:'/'},
  {name:'gallery', href: '/'}
]
</script>

<header class="max-w-full bg-amber-700 ">
  <div class="p-2 mx-2 ">
    <img class="max-w-[25px] max-h-[25px] hover:bg-amber-400 hover:rounded-full" src="./logo.svg" alt="pot on stove">
  </div>
  <nav class="max-w-fit text-white">
    <ul class="flex justify-around">
      {#each navItems as {name , href}}
      <a {href}><li>{name}</li></a>
      {/each}
    </ul>
  </nav>
</header>