<script>
</script>

<!--HTML-->
<div class="container">
  <h2>Enter a new record:</h2>
  <div class="record">
    <label for="date"
      >Date
      <input type="date" id="date" />
    </label>

    <label for="sales"
      >$ Sales
      <input type="number" id="sales" />
    </label>

    <label for="labor"
      >$ Labor
      <input type="date" />
    </label>
    <div class="labor-percent">
      <h3>Labor %</h3>
      <p class="labor-output">Test</p>
    </div>
  </div>
</div>

<!--CSS-->
<style>
  .container {
  }
  label,
  .labor-percent {
    display: flex;
    flex-direction: column;
    width: 15%;
  }
</style>
