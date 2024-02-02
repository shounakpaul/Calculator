<script>
  let num1 = 0;
  let num2 = 0;
  let result = 0;

  function add() {
    result = num1 + num2;
  }

  function subtract() {
    result = num1 - num2;
  }

  function multiply() {
    result = num1 * num2;
  }

  function divide() {
    result = num1 / num2;
  }
</script>

<main>
  <h1>Calculator</h1>

  <input type="number" bind:value={num1} />
  <input type="number" bind:value={num2} />

  <button on:click={add}>Add</button>
  <button on:click={subtract}>Subtract</button>
  <button on:click={multiply}>Multiply</button>
  <button on:click={divide}>Divide</button>

  <p>Result: {result}</p>
</main>
