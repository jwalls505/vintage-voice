<script>
  import { onMount } from 'svelte';
</script>

<div class="page-content">
  <div class="card">
    <h1>Demo Reel</h1>
    <audio controls class="audio-player" src="/demoReel/voiceDemo.mp3">
      Your browser does not support the audio element.
    </audio>
  </div>
</div>

<style>
  .audio-player {
    width: 100%;
    margin-top: 2rem;
  }
</style>
