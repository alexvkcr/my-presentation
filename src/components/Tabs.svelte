<script>
  import Tab from "./Tab.svelte";
  import { createEventDispatcher } from "svelte";
  import Delayed from "./Delayed.svelte";
</script>

<div class="tabs">
  <Delayed waitInMili={500}>
    <Tab tabName="My CV" specialHover="true"/>
  </Delayed>
  <Delayed waitInMili={1500}>
    <Tab tabName="My Projects" specialHover="true"/>
  </Delayed>
  <Delayed waitInMili={2500}>
    <Tab tabName="Testimonials" specialHover="true"/>
  </Delayed>
  <Delayed waitInMili={3500}>
    <Tab tabName="Contact me" specialHover="true"/>
  </Delayed>
  <Delayed waitInMili={4500}>
    <Tab type="last-item" tabName="Night mode" />
  </Delayed>
</div>

<style>
  .tabs {
    width: calc(100% - 20px);
    height: 50px;
    padding: 20px;

    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    align-items: baseline;
  }
</style>
