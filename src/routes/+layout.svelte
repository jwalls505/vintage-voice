<script lang="ts">
	import '../app.css';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href="/pics/VintageVoice-Emblem.png" />
</svelte:head>

<header class="header">
  <nav class="nav">
    <a href="/" class="logo-area">
      <img src="/pics/VintageVoice-Emblem.png" alt="The Vintage Voice Emblem" class="emblem" />
      <div class="logo-container">
        <span class="logo">The Vintage Voice</span>
        <p class="subtitle">Engineer-Artist-Advocate</p>
      </div>
    </a>
    <ul class="nav-links">
      <li><a href="/bio">BIO</a></li>
      <li><a href="/work">WORK</a></li>
      <li><a href="/info-rates">INFO & RATES</a></li>
      <li><a href="/contact">CONTACT</a></li>
    </ul>
  </nav>
</header>

<main>
  {@render children?.()}
</main>

<footer class="footer">
  <p>&copy; 2025 The Vintage Voice</p>
</footer>

<style>
  .logo-area {
    display: flex;
    align-items: center;
    gap: 1.5rem; /* Adjust space between emblem and text */
    text-decoration: none; /* Removes underline from the new link wrapper */
  }

  .emblem {
    height: 120px; /* Adjust size as needed */
    width: auto;
  }

  .logo-container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .subtitle {
    font-family: var(--heading-font);
    font-size: 1.2rem;
    color: var(--text-color);
    margin: 0;
    letter-spacing: 0.05em;
  }

  .footer {
    text-align: center;
    padding: 2rem 0;
    margin-top: 4rem;
    border-top: 1px solid #eee;
    color: #777;
    font-size: 0.9rem;
  }
</style>
