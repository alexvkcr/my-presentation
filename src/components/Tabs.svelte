<script>
  import Tab from "./Tab.svelte";
</script>

<div class="tabs">
  <Tab tabName="Me" />
  <Tab tabName="My CV" />
  <Tab tabName="My Projects" />
  <Tab tabName="Contact me" />
  <Tab class="last-item" tabName="Fashion mode" />
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
  .last-item {
    order: 4; /* default is 0 */
    color: red;
  }
</style>
