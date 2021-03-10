<script>
  import Tab from "./Tab.svelte";
  import { createEventDispatcher } from "svelte";
</script>

<div class="tabs">
  <Tab tabName="My CV" />
  <Tab tabName="My Projects" />
  <Tab tabName="Testimonials" />
  <Tab tabName="Contact me" />
  <Tab type="last-item" tabName="Fashion mode" />
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
