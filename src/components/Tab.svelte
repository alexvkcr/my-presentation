<script>
  export let tabName = "";
</script>

<h1>{tabName}!</h1>

<style>
  h1 {
    display: inline-block;
    margin: 0 10px;
  }

  @media (max-width: 600px) {
    h1 {
      margin: 20px 10px;
    }
  }
  @media (max-width: 800px) {
    h1 {
      margin: 25px 10px;
    }
  }
</style>
