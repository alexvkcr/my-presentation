<script>
  import { onMount } from "svelte";

  export let waitInMili = 500;
  let shown = false;

  onMount(() => setTimeout(() => (shown = true), waitInMili));
</script>

{#if shown}
  <slot />
{/if}

<style></style>
