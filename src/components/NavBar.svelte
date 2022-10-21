<script>
  // @ts-nocheck
  history.scrollRestoration = "manual" // Prevent automatic scrolling
  const navItems = [
    { title: "About", url: "#About" },
    { title: "Experiences", url: "#Experiences" },
    { title: "Projects", url: "#Projects" },
  ];
  let time = new Date(Date.now());
  const options = {
    weekday: "long",
  };
</script>

<nav>
  <section class="container__nav" id="/">
    <ol class="container__nav" id="/">
      {#each navItems as { title, url }}
        <li>
          <a href={url} class="nav__item">
            {title}
          </a>
        </li>
      {/each}
    <p class="time">{time.toLocaleDateString(undefined, options)}</p>
  </ol>
  </section>
</nav>

<style>
   ol {
    list-style: none;
  }
  li {
    padding: 0;
  }
  .container__nav {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
  }
  .nav__item {
    color: white;
    font-weight: 600;
    font-size: 2rem;
    margin: 0 2rem;
    transition: all 400ms;
  }
  .nav__item:hover {
    color: rgb(0, 157, 255);
  }
  .time {
    color: #1a1a1a;
    font-weight: 700;
    background-color: #2C91C6;;
    padding: 0.35rem;
    margin: 0 2rem;
    border-radius: 12px;
  }
</style>
