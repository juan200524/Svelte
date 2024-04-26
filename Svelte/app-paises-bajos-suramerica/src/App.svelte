<script>
  import Paises from "./lib/países.svelte";
  const lista=["colombia","venezuela","ecuador","peru","brasil","argentina","chile","guyana","paraguay","surinam","uruguay"]
</script>

  <div class="main">
    {#each lista as pais}
      <div>
      <Paises {pais}/>
        </div>
      {:else}
      no existen elementos
      
    {/each}
  </div>
  <svelte:head>
    <title> paises de suramerica</title>
  </svelte:head>

<style>
  .main{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid: gad 10px;
    grid-auto-rows: minmax(100px, auto);
  }
 
</style>
