<svelte:options runes />

<script>
  let name = "Wecisankonde"; // Personalized name
  let message = "You are strong, capable, and loved. Keep shining your light!";
  let from = "Love of Your Life"; // Who it's from
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>{message}</p>
  <p> With love, {from} d</p>

  <label for="nameInput">Want to personalize it?</label>
  <input id="nameInput" bind:value={name} placeholder="Type your name..." />
</main>

<style>
  main {
    text-align: center;
    margin-top: 50px;
    font-family: Arial, sans-serif;
  }
  h1 {
    color: #ff4081;
  }
  p {
    font-size: 18px;
    color: #333;
  }
  input {
    padding: 10px;
    font-size: 16px;
    margin-top: 10px;
  }
</style>
<h1>Hello {name}!</h1>
