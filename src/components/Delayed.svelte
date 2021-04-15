<script>
  import { onMount } from "svelte";

  export let waitInMili = 500;
  let shown = false;

  onMount(() => setTimeout(() => (shown = true), waitInMili));
</script>

<div class:hidden={!shown}>
  <slot />
</div>

<style>
  div {
    visibility: visible;
    opacity: 1;
    transition: visibility 0.8s linear, opacity 0.8s linear;
  }
  .hidden {
    visibility: hidden;
    opacity: 0;
  }
</style>
