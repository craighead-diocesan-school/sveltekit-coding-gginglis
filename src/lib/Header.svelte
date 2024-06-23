<div class="banner">
  <header class="hero">
    <div class="hero-body">
      <h1 class="title">Welcome</h1>
      <h2 class="subtitle">Welcome to my site</h2>
    </div>
  </header>

  <nav>
    <a href="/">home</a>
    <a href="/input output">input output</a>
    <a href="/selection">selection</a>
    <a href="/iteration">iteration</a>
  </nav>
</div>

<style>
  h1,
  h2 {
    font-family: "Red Hat Display", sans-serif;
    font-weight: 900;
    color: rgb(38, 41, 116);
  }

  h1 {
    font-size: 2.3rem;
  }
  nav {
    display: flex;
    flex-direction: row;
    margin: 60px 30px 50px 600px;
  }

  a {
    margin: 15px;
    font-family: "Red Hat Display", sans-serif;
    font-weight: 900;
    font-size: 1.3rem;
    color: rgb(38, 41, 116);
    transition: 0.3s;
  }

  a:hover {
    color: rgba(38, 41, 116, 0.658);
    transition: 0.3s;
  }

  .banner {
    display: flex;
  }
</style>
