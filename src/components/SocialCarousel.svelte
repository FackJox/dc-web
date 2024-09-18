<script>
  const socialMedia = [
    { name: 'TikTok', icon: 'tiktok', url: 'https://www.tiktok.com/@drum.cult' },
    { name: 'Instagram', icon: 'instagram', url: 'https://www.instagram.com/drum.cult' },
    { name: 'YouTube', icon: 'youtube', url: 'https://www.youtube.com/@DrumCult' },
    { name: 'SoundCloud', icon: 'soundcloud', url: 'https://soundcloud.com/drumcultevents' },
  ];
</script>

<div class="social-container">
  {#each socialMedia as item}
    <a href={item.url} target="_blank" rel="noopener noreferrer" class="social-icon">
      <i class="fab fa-{item.icon}"></i>
      <span class="tooltip">{item.name}</span>
    </a>
  {/each}
</div>

<style>
  .social-container {
    display: flex;
    flex-direction: row;
    gap: 1vw;
    align-items: center;
    justify-content: flex-end;
    width: 100%;
    height: 100%;
  }

  .social-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 5vw;
    height: 5vw;
    min-width: 40px;
    min-height: 40px;
    max-width: 80px;
    max-height: 80px;
    background-color: #d9d9d9;
    color: black;
    border-radius: 50%;
    text-decoration: none;
    font-size: calc(1rem + 1vw);
    transition: transform 0.3s ease, background-color 0.3s ease;
    position: relative;
    box-shadow: 0px 2px 2px 0px rgba(0, 0, 0, 0.25);
  }

  .social-icon:hover {
    transform: scale(1.1);
    background-color: #bfbfbf;
  }

  .tooltip {
    position: absolute;
    top: -30px;
    left: 50%;
    transform: translateX(-50%);
    background-color: rgba(0, 0, 0, 0.7);
    color: white;
    padding: 5px 10px;
    border-radius: 5px;
    font-size: 0.8rem;
    opacity: 0;
    transition: opacity 0.3s ease;
    pointer-events: none;
    white-space: nowrap;
  }

  .social-icon:hover .tooltip {
    opacity: 1;
  }

  @media (max-width: 768px) {
    .social-container {
      justify-content: center;
    }

    .social-icon {
      width: 8vw;
      height: 8vw;
    }
  }

  @media (max-width: 480px) {
    .social-icon {
      width: 10vw;
      height: 10vw;
    }
  }
</style>