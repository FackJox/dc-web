<script>
  import Event from './Event.svelte';
</script>

<main>
  <Event />
  <div class="embrace">Embrace</div>
  <div class="the-cult-container">
     <div class="the-cult">THE CULT</div>
     <div class="let-s-dance-together">Let's Oscillate Together</div>
  </div>
</main>

<a href="https://www.skiddle.com/whats-on/Bristol/Box-7/DrumCult-The-Initiation/40037719/" style="text-decoration: none; color: inherit;">
  <div class="frame-8">
    <div class="frame-7">
      <div class="initiation-w-matt-scratch-pcilocybin-laden">
        INITIATION: w/ Matt Scratch &amp; Pcilocybin Laden
      </div>
      <div class="date">28.09.2024</div>
    </div>
  </div>
</a>


<style>
  main {
      position: relative;
      width: 100vw;
      height: 100vh;
      overflow: hidden;
  }

  .creative-community {
      color: #ffffff;
      text-align: left;
      font-family: "Poppins-Regular", sans-serif;
      font-size: 1.5vw;
      font-weight: 400;
      position: absolute;
      left: 8vw;
      bottom: 5vh;
  }

  

  .the-cult-container {
      position: absolute;
      left: 52.5vw;
      top: 50vh;
      transform: translate(-25%, -50%);
  }

  .the-cult {
      color: #e1e1e1;
      text-align: left;
      font-family: "Poppins-Bold", sans-serif;
      font-size: 8vw;
      font-weight: 700;
      text-transform: uppercase;
      white-space: nowrap;
  }

  .let-s-dance-together {
      color: #ffffff;
      text-align: left;
      font-family: "Poppins-Regular", sans-serif;
      font-size: 2vw;
      font-weight: 400;
      position: absolute;
      left: 20vw;
      top: 16vh;
      white-space: nowrap;
  }

  .embrace {
      color: #e1e1e1;
      text-align: left;
      font-family: "Poppins-Bold", sans-serif;
      font-size: 10vw;
      font-weight: 700;
      text-transform: uppercase;
      position: absolute;
      left: 47.5vw;
      top: 30vh;
      transform: translate(-75%, -50%);
      white-space: nowrap;
  }
</style>