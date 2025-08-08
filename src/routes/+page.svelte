<script>
  import Table from '../lib/Table.svelte'
  let { data } = $props()

  console.log(data)
</script>

<main
  class="relative flex flex-col items-center justify-center min-h-screen py-10"
>
  
  <h1
    class="pt-4 pb-8 bg-gradient-to-br dark:from-white from-black via-[#707070] to-[#ffffff] bg-clip-text text-center text-4xl font-medium tracking-tight text-transparent md:text-7xl"
  >
    Supabase x sveltekit
  </h1>
   <ul>
    {#each data.instruments as instrument}
      <li>{instrument.name}</li>
    {/each}
  </ul>
 
</main>


