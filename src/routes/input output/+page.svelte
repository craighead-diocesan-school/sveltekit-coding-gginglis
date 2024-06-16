<script>
  import Header from "$lib/Header.svelte";
  import Nav from "$lib/Nav.svelte";
  let usd = 0;
  let nzd = usd * 1.6248;
  let roundedNzd = nzd.toFixed(2);
  function converter() {
    nzd = usd * 1.62;
    roundedNzd = nzd.toFixed(2);
  }
  // let name = "world";
  // import ImageCard from "$lib/ImageCard.svelte";
  // let selectedOption = "Option 1";
  // let count = 0;

  // function increment() {
  //   count = count + 1;
  // }

  // import HiButton from "../lib/HiButton.svelte";
</script>

<!-- <input bind:value={name} placeholder="Enter your name" />
<select bind:value={selectedOption}>
  <option value="Option 1">Option 1</option>
  <option value="Option 2">Option 2</option>
  <option value="Option 3">Option 3</option>
</select> -->

<Header />

<Nav />
<main>
  <h2>currency converter</h2>
  <p>NZD: ${roundedNzd}</p>
  <input bind:value={usd} placeholder="Enter price in USD" />
  <button on:click={converter}></button>
  <!-- <h1>Hello {name}!</h1>
  <h2>SvelteKit</h2> -->

  <!-- <p>You selected: {selectedOption}</p> -->

  <!-- <p>Count: {count}</p>
  <button on:click={increment}>Increment</button> -->

  <!-- <ImageCard />
    
    <HiButton /> -->

  <!-- <p>
      Welcome to coding with SvelteKit, a modern JavaScript framework that makes
      it easy to code great apps.
    </p> -->
</main>

<footer>
  <p>&copy; Craighead Diocesan School 2024</p>
</footer>

<style>
  button {
    width: 1rem;
    height: 1rem;
  }

  h2 {
    font-weight: bold;
  }

  main {
    margin-left: 30px;
  }
</style>
