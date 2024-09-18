<script>
  const navItems = ['Home', 'Events', 'About', 'Contact'];
</script>

<nav>
  <div class="logo">DrumCult</div>
  <ul>
    {#each navItems as item}
      <li><a href="#{item.toLowerCase()}">{item}</a></li>
    {/each}
  </ul>
</nav>

<style>
  nav {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 2rem;
    background-color: rgba(0, 0, 0, 0.0);
    z-index: 10;
  }

  .logo {
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
  }


  ul {
    display: flex;
    list-style-type: none;
    margin: 0;
    margin-right: 2rem;
    padding: 0;
    color: white;
    font-size: 1.5rem;
  }

  li {
    margin-left: 1rem;
  }

  a {
    color: white;
    text-decoration: none;
  }
</style>