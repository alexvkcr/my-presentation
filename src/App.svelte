<script>
  import Router from "svelte-spa-router";

  import Tabs from "./components/Tabs.svelte";
  import Error from "./components/Error.svelte";
  import Delayed from "./components/Delayed.svelte";
  import Ocean from "./components/Ocean.svelte";
  import Stage from "./components/Stage.svelte";

  const routes = {
    "/": Tabs,
    "*": Error,
  };
</script>

<Router {routes} />
<Delayed waitInMili={3500}>
  <Stage />
</Delayed>
<Delayed waitInMili={2500}>
  <Ocean />
</Delayed>

<style>
</style>
