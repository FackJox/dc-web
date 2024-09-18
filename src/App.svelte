<script>
  import Header from './components/Header.svelte';
  import BackgroundContainer from './components/BackgroundContainer.svelte';
  import ForegroundContainer from './components/ForegroundContainer.svelte';
  import SocialCarousel from './components/SocialCarousel.svelte';
</script>

<main>
  <BackgroundContainer />
  <div class="overlay-image"></div>
  <div class="content-wrapper">
    <Header />
    <ForegroundContainer />
  </div>
  <div class="social-carousel-wrapper">
    <SocialCarousel />
  </div>
</main>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
  }

  main {
    position: relative;
    width: 100vw;
    height: 100vh;
    overflow: hidden;
  }

  .overlay-image {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    /* background-image: url('https://via.placeholder.com/1920x1080'); */
    background-size: cover;
    background-position: center;
    opacity: 0.5;
    z-index: 1;
  }

  .content-wrapper {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 2;
    display: flex;
    flex-direction: column;
  }

  .social-carousel-wrapper {
    position: absolute;
    bottom: 4vh;
    right: 5vw;
    z-index: 3;
    max-width: 50vw;
    max-height: 30vh;
  }

  @media (max-width: 768px) {
    .social-carousel-wrapper {
      max-width: 80vw;
      max-height: 20vh;
    }
  }
</style>