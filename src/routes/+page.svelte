<script>
  import Header from "$lib/Header.svelte";
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

<main>
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

  /* button {
    width: 5rem;
    height: 5rem;
    margin: 3rem 3rem;
    border: none;
    border-radius: 25px;
    background: linear-gradient(145deg, #cacaca, #f0f0f0);
    box-shadow:
      10px 10px 30px #bebebe,
      -10px -10px 30px #ffffff;
  } */
</style>
