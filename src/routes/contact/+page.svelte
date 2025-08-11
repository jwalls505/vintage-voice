<script>
  import { onMount } from 'svelte';
</script>

<div class="page-content">
  <div class="card">
    <h1>Contact</h1>
    <form class="card">
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" required>
      </div>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
      </div>
      <div class="form-group">
        <label for="message">Message</label>
        <textarea id="message" name="message" required></textarea>
      </div>
      <button type="submit">Send Message</button>
    </form>
  </div>
</div>

<style>
  .form-group {
    margin-bottom: 1.5rem;
    text-align: left;
  }

  label {
    display: block;
    margin-bottom: 0.5rem;
    font-family: var(--body-font);
    font-weight: bold;
  }

  input,
  textarea {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-family: var(--body-font);
    font-size: 1rem;
  }

  textarea {
    min-height: 150px;
    resize: vertical;
  }

  button {
    display: inline-block;
    padding: 0.8rem 2rem;
    background-color: var(--title-bg-color);
    color: #fff;
    font-family: var(--heading-font);
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  button:hover {
    background-color: #a9862e; /* A slightly darker gold for hover */
  }
</style>
