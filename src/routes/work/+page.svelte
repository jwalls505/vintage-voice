<script>
  import { onMount } from 'svelte';

  const projects = [
    { image: '/pics/work/avets.png', title: 'Project Title 1', description: 'A brief description of the project.' },
    { image: '/pics/work/chase_marketing.png', title: 'Project Title 2', description: 'A brief description of the project.' },
    { image: '/pics/work/luxlab.png', title: 'Project Title 3', description: 'A brief description of the project.' },
    { image: '/pics/work/sewing_for_angels.png', title: 'Project Title 4', description: 'A brief description of the project.' },
    { image: '/pics/work/young_living.png', title: 'Project Title 5', description: 'A brief description of the project.' },
    { image: '/pics/work/shriners.png', title: 'Project Title 6', description: 'A brief description of the project.' },
    { image: '/pics/work/bam_marketing.png', title: 'Project Title 7', description: 'A brief description of the project.' },
    { image: '/pics/work/hifi3d.png', title: 'Project Title 8', description: 'A brief description of the project.' },
    { image: '/pics/work/kissofwar.png', title: 'Project Title 9', description: 'A brief description of the project.' },
    { image: '/pics/work/tap4fun.png', title: 'Project Title 9', description: 'A brief description of the project.' },
    { image: '/pics/work/crealon.png', title: 'Project Title 9', description: 'A brief description of the project.' },
    { image: '/pics/work/fortunecookiewisdom.png', title: 'Project Title 9', description: 'A brief description of the project.' },
    
  ];
</script>

<div class="page-content">
  <div class="card">
    <h1>Clients/Testimonials</h1>
    <div class="work-grid">
      {#each projects as project, i}
        <div class="card project-card">
          <div class="image-wrapper">
            <img src="{project.image}" alt="{project.title}" class="project-image" />
          </div>
          <!-- <div class="project-content">
            <h2>{project.title}</h2>
            <p>{project.description}</p>
          </div> -->
        </div>
      {/each}
    </div>
  </div>
</div>

<style>
  .work-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .project-card {
    overflow: hidden; /* Ensures the image corners are clipped correctly */
    padding: 0; /* Remove default card padding */
    display: flex;
    flex-direction: column;
    background-color: #fff; /* Ensure card has a background */
    border: 1px solid #eee;
  }

  .image-wrapper {
    aspect-ratio: 3 / 2; /* Use a responsive aspect ratio instead of fixed height */
    padding: 1rem; /* Space around the logo */
    background-color: #f8f9fa; /* A very light gray background */
    display: flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
  }

  .project-image {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain; /* This ensures the whole image is visible */
    display: block;
  }

  .project-content {
    padding: 1.5rem;
  }

  .project-content h2 {
    font-size: 1.8rem;
    margin-bottom: 0.5rem;
    text-transform: none;
    letter-spacing: normal;
    font-weight: 700;
  }
</style>
