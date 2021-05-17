<script>
  import Tab from "./Tab.svelte";
  import { createEventDispatcher } from "svelte";
  import Delayed from "./Delayed.svelte";
  import Hover from "./Hover.svelte";
</script>

<div class="tabs">
  <Delayed waitInMili={500}>
    <Hover>
      <Tab tabName="My CV" />
    </Hover>
  </Delayed>
  <Delayed waitInMili={1500}>
    <Hover>
      <Tab tabName="My Projects" />
    </Hover>
  </Delayed>
  <Delayed waitInMili={2500}>
    <Hover>
      <Tab tabName="Testimonials" />
    </Hover>
  </Delayed>
  <Delayed waitInMili={3500}>
    <Hover>
      <Tab tabName="Contact me" />
    </Hover>
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
