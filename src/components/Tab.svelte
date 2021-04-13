<script>
  export let tabName = "";
  export let type = "normal";

  function fashionMode(e) {
    if (e.target.outerText == "Fashion mode") {
      console.log("clicked fashion Mode");
    }
  }
</script>

<h1 class={type === "last-item" ? "last-item" : ""} on:click={fashionMode}>
  {tabName}
</h1>

<style>
  h1 {
    display: inline-block;
    margin: 0 10px;
  }

  .last-item {
    order: 4; /* default is 0 */
    color: red;
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
