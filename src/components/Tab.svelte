<script>
  import Hover from "./Hover.svelte";

  export let tabName = "";
  export let specialHover = false;
  export let type = "normal";

  function fashionMode(e) {
    if (e.target.outerText == "Fashion mode") {
      console.log("clicked fashion Mode");
    }
  }
</script>

{#if specialHover}
  <Hover>
    <h1 class={type === "last-item" ? "last-item" : ""} on:click={fashionMode}>
      {tabName}
    </h1>
  </Hover>
  {:else}
  <h1 class={type === "last-item" ? "last-item" : ""} on:click={fashionMode}>
    {tabName}
  </h1>
{/if}

<style>
  h1 {
    display: inline-block;
    margin: 0 10px;
  }

  .last-item {
    order: 4; /* default is 0 */

    padding: 0 0.6em;

    color: white;
    background-color: black;
    
    border: 4px solid grey;
    border-color: grey;
    border-radius: 7px;
    
    transition: 1.0s;
  }

  .last-item:hover {
    color: black;
    background-color: lightgrey;

    border: 4px solid yellow;
  }

  @media (max-width: 600px) {
    h1 {
      margin: 20px 10px;
    }
  }
  @media (max-width: 800px) {
    h1 {
      margin: 25px 10px;
    }
  }
</style>
