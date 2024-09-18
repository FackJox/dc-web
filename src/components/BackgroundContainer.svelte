<script>
  import RedBackground from './RedBackground.svelte';
  import BlueBackground from './BlueBackground.svelte';
</script>

<div class="background-container">
  <RedBackground />
  <BlueBackground />
</div>

<style>
  .background-container {
    display: flex;
    width: 100%;
    height: 100%;
  }

  @media (max-width: 768px) {
    .background-container {
      flex-direction: column;
    }
  }
</style>