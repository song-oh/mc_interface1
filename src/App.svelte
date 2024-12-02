<script>
  import Model from "./Model.svelte";
  import Dataset from "./Dataset.svelte";
  import Bar from "./Bar.svelte";
  import Predictors from "./Predictors.svelte";
</script>

<div class="container">
  <div class="left">
    <Model />
    <Dataset />
  </div>
  <div class="right">
    <Bar />
    <Predictors />
  </div>
</div>

<style>
  .container {
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 1rem;
    height: 100vh;
    overflow: hidden;
  }

  .left {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }

  .right {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    overflow-y: auto;
  }
</style>
