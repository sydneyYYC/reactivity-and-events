<script>
export const navItems = [
  {name:'recipies', href:'/'},
  {name:'gallery', href: '/'}
]
</script>

<header class="max-w-full bg-amber-700 flex justify-between items-center">
  <div class="p-2 mx-2 min-w-[50px] min-h-[30px]">
    <img class="max-w-[30px] max-h-[30px] hover:bg-amber-400 hover:rounded-full" src="./logo.svg" alt="pot on stove">
  </div>
  <nav class="max-w-fit text-white">
    <ul class="flex justify-around self-end">
      {#each navItems as {name , href}}
      <a {href}><li class="mx-4 mr-2 my-2 hover:bg-amber-400 p-2 hover:rounded-full">{name}</li></a>
      {/each}
    </ul>
  </nav>
</header>