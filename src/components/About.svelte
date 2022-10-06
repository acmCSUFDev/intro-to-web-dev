<script>
  export let name;
  import frank from "../assets/frank.svg";
</script>

<section>
  <div class="container__about" id="About">
    <img width={180} height={123} src={frank} alt="" />
    <p class="header__about--small">Hi, I'm {name}</p>
    <p class="header__about--big">WELCOME TO MY PORTFOLIO</p>
  </div>
</section>

<style>
  .container__about {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10rem;
  }
  .header__about--small {
    font-size: 1.5rem;
    margin: 2rem 0 0 0;
    font-weight: 600;
  }

  .header__about--big {
    font-size: 2rem;
    color: #2C91C6;
    font-weight: 700;
  }
</style>
