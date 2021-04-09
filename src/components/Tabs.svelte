<script>
  import Tab from "./Tab.svelte";
  import { createEventDispatcher } from "svelte";
  import DelayedVisible from "./DelayedVisible.svelte";
</script>

<div class="tabs">
  <DelayedVisible waitInMili={1000}>
    <Tab tabName="My CV" />
  </DelayedVisible>
  <DelayedVisible waitInMili={2000}>
    <Tab tabName="My Projects" />
  </DelayedVisible>
  <DelayedVisible waitInMili={3000}>
    <Tab tabName="Testimonials" />
  </DelayedVisible>
  <DelayedVisible waitInMili={4000}>
    <Tab tabName="Contact me" />
  </DelayedVisible>
  <DelayedVisible waitInMili={6000}>
    <Tab type="last-item" tabName="Fashion mode" />
  </DelayedVisible>
</div>

<style>
  .tabs {
    width: calc(100% - 20px);
    height: 50px;
    margin: 20px;

    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    align-items: baseline;
  }
</style>
