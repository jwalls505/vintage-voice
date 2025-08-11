<script>
  import { onMount } from 'svelte';
</script>

<div class="page-content">
  <h1 class="page-title">About Me</h1>
  <div class="bio-container">
    <div class="left-column">
      <img src="/pics/Headshot.jpeg" alt="Headshot" class="bio-image" />
      <div class="equipment-section">
        <h3 class="equipment-title">Equipment—</h3>
        <p>Microphone-Shure PGA27</p>
        <p>Interface-Scarlett 4i4</p>
        <p>Software-ProTools 11</p>
        <p>Source-Connect Standard</p>
      </div>
    </div>
    <div class="right-column">
      <p>
        I have had an interest in voice over for almost as long as I have been in love with all things vintage! At my
        core, I knew this is what I wanted to do with my life, and after many years of trying other avenues, everything
        led back to the mic!
      </p>
      <p>
        Passion is at the root of every endeavor, and it is my job to bring Your passion to the world. I can confidently
        perform with a vocal age range from child to 35 years old with an assortment of dialects. (In true vintage form,
        I can even speak a little Latin!) You're welcome to ask for any sound and I'll be willing to explore and
        collaborate!
      </p>
      <p>
        In September of 2020, I completed a post-graduate program in Audio Engineering and Production under the
        mentorship of Grammy-winning, Hollis Greathouse.
      </p>
      <p>
        With my home studio, I am able to record, mix, and master broadcast quality work. You may even direct me via
        phone call, GoogleMeet, or Zoom!
      </p>
    </div>
  </div>
</div>

<style>
  .page-title {
    font-family: var(--heading-font);
    font-size: 3.5rem;
    color: var(--title-bg-color);
    text-align: left;
    margin-bottom: 2rem;
    /* Override global h1 styles */
    background-color: transparent;
    padding: 0;
    text-transform: none;
    letter-spacing: normal;
    font-weight: normal;
    position: static;
  }

  .page-title::after {
    display: none; /* Hide the decorative line from global styles */
  }

  .bio-container {
    display: flex;
    gap: 3rem;
    align-items: flex-start;
  }

  .left-column {
    flex: 0 0 350px; /* Set a fixed width for the left column */
  }

  .right-column {
    flex: 1;
  }

  .bio-image {
    width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  }

  .equipment-section {
    margin-top: 2rem;
  }

  .equipment-title {
    font-family: var(--heading-font);
    font-size: 2rem;
    color: var(--title-bg-color);
    margin-bottom: 0.5rem;
    font-weight: normal;
  }

  .equipment-section p {
    font-family: var(--body-font);
    font-style: italic;
    color: #555;
    margin: 0.25rem 0;
    line-height: 1.5;
  }

  .right-column p {
    margin-bottom: 1.5rem;
    font-family: var(--body-font);
    font-style: italic;
  }
</style>
