<script lang="ts">
  let count: number = 0;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -= 1;
  }
</script>

<style>
main {
    text-align: center;
    margin: 50px;
  }

  h1 {
    font-size: 2em;
    margin-bottom: 20px;
  }

  button {
    font-size: 1em;
    padding: 10px 20px;
    margin: 0 10px;
    cursor: pointer;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 4px;
  }

  button:hover {
    background-color: #45a049;
  }

  button:active {
    background-color: #3e8e41;
  }
</style>

<main>
  <h1>Counter : {count}</h1>
  <button on:click={increment}>Increment</button>
  <button on:click={decrement}>Decrement</button>
</main>

