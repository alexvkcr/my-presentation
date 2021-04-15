<script>
  import Tabs from "./components/Tabs.svelte";
  import Delayed from "./components/Delayed.svelte";
</script>

<Tabs />
<Delayed waitInMili={2500}>
  <div class="img-container">
    <img src="/img/alexWeb.gif " alt="foto del autor, Alejandro" />
  </div>
</Delayed>

<style>
  .img-container {
    display: flex;
    justify-content: center;
  }
  img {
    width: 45vw;
  }
</style>
