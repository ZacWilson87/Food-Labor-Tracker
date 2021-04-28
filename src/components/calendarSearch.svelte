<script>
  let choice = "";
</script>

<main>
  <div class="view-by-container">
    <h2>View By</h2>

    <label for="viewByChoice" />
    <select name="viewByChoice" id="viewByChoice" bind:value={choice}>
      <option value="" disabled select hidden>Select</option>
      <option value="date">Day</option>
      <option value="week">Week</option>
      <option value="month">Month</option>
    </select>

    {#if !choice}
      <input type={choice} style="display: none" />
    {/if}
    {#if choice}
      <input type={choice} />
    {/if}
  </div>
</main>

<style>
  .view-by-container {
    justify-content: center;
    align-items: center;
    text-align: center;
    display: flex;
    flex-direction: column;
  }
  h2 {
    color: rgb(194, 194, 194);
  }
  input {
    text-align: center;
  }
  select,
  option {
    width: 10%;
    text-align: center;
    margin: 1%;
    border-radius: 0.25em;
  }
</style>
