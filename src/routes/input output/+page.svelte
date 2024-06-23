<script>
  import Header from "$lib/Header.svelte";
  let usd = 0;
  let nzd = usd * 1.6344;
  let roundedNzd = nzd.toFixed(2);
  function converter() {
    nzd = usd * 1.6344;
    roundedNzd = nzd.toFixed(2);
  }
  import Footer from "$lib/Footer.svelte";
</script>

<Header />

<main>
  <h2>currency converter</h2>
  <p>NZD: ${roundedNzd}</p>
  <input bind:value={usd} placeholder="Enter price in USD" />
  <button on:click={converter}>enter</button>
</main>

<Footer />

<style>
  button {
    /* width: 1.2rem;
    height: 1.2rem; */
    border: solid rgb(38, 41, 116) 3px;
    background-color: rgb(130, 132, 181);
    transition: 0.15s;
    font-family: "Red Hat Display", sans-serif;
    color: rgb(38, 41, 116);
    /* font-weight: 300; */
  }

  button:hover {
    background-color: rgb(60, 62, 132);
    transition: 0.15s;
  }

  h2 {
    font-weight: bold;
    font-size: 1.7rem;
    color: rgb(38, 41, 116);
    font-family: "Red Hat Display", sans-serif;
    margin-bottom: 5px;
  }
  p {
    font-weight: 600;
    font-size: 1.3rem;
    color: rgb(38, 41, 116);
    font-family: "Red Hat Display", sans-serif;
    margin-bottom: 7px;
  }
  input {
    border: solid rgb(38, 41, 116) 3px;
  }
  main {
    margin-left: 50px;
  }
</style>
