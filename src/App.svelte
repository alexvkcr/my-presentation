<script>
  import Router from "svelte-spa-router";

  import Tabs from "./components/Tabs.svelte";
  import Error from "./components/Error.svelte";
  import Delayed from "./components/Delayed.svelte";

  const routes = {
    "/": Tabs,
    "*": Error,
  };
</script>

<Router {routes} />

<style>
</style>
