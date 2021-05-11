<script>
  import Tab from "./Tab.svelte";
  import { createEventDispatcher } from "svelte";
  import Delayed from "./Delayed.svelte";
</script>

<div class="tabs">
  <Delayed waitInMili={500}>
    <Tab tabName="My CV" />
  </Delayed>
  <Delayed waitInMili={1500}>
    <Tab tabName="My Projects" />
  </Delayed>
  <Delayed waitInMili={2500}>
    <Tab tabName="Testimonials" />
  </Delayed>
  <Delayed waitInMili={3500}>
    <Tab tabName="Contact me" />
  </Delayed>
  <Delayed waitInMili={4500}>
    <Tab type="last-item" tabName="Night mode" />
  </Delayed>
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
