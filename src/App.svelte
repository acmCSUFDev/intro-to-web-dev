<script>
  import About from "./components/About.svelte";
  import Experiences from "./components/Experiences.svelte";
  import NavBar from "./components/NavBar.svelte";
  import Projects from "./components/Projects.svelte";
</script>

<main>
  <div>
    <NavBar />
    <About name={"Frank"} />
    <Experiences />
    <Projects/>
  </div>
</main>

<style>
  main {
    margin: 1rem;
    font-size: 1.25rem;
  }
</style>
