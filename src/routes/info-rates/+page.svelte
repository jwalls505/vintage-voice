<script>
  import { onMount } from 'svelte';
</script>

<div class="page-content">
  <div class="card">
    <h1>Info & Rates</h1>
    <div class="rates-content">
      <p>
        With the ever-growing and changing world of voice over, rates are constantly evolving. My studio rates are
        fixed, but usage fees are negotiable based on distribution. To get an idea of the industry standard, please
        visit the <a href="https://globalvoiceacademy.com/gvaa-rate-guide-2/" target="_blank">GVAA Rate Guide</a>.
      </p>

      <h3>Before I can offer a quote, I will need the following information:</h3>
      <ul>
        <li>The copy/script length (in 00:00 for Commercial, in word count for Narration)</li>
        <li>Intended usage (Digital, TV, Radio, etc.)</li>
        <li>Term (How long it will be in use or if you prefer total buyout)</li>
        <li>If your project is a one-off or part of a series</li>
        <li>If there are any character/dialectical requirements</li>
        <li>Your deadline</li>
      </ul>

      <p>
        Please keep in mind that finely-tuned crisp editing comes standard in my final product, which takes time as
        well. Commercial projects come standard with unlimited revisions for one week after delivery.
      </p>

      <p>
        Make sure that the copy you send contains no errors - I offer language editing services for overseas clientele.
        I read EXACTLY what's on the script.
      </p>

      <h3>Please consider/avoid:</h3>
      <ul>
        <li>Run-on sentences as I need to be able to breathe. :)</li>
        <li>Grammatical or syntactical errors</li>
        <li>Specify acronyms (e.g., "ACT" or "A See Tee")</li>
        <li>Specify conjunctions involving "/"s that may be spoken as "or", "per", etc.</li>
      </ul>

      <p>
        Let me know of any retakes (due to performance, pace, tone) you would like to make within one week after
        delivery. Re-takes due to script errors or minor script changes will incur a charge. Major re-writes due to
        consistent errors (as listed above) constitute a new project and warrants an additional session fee.
      </p>

      <p>
        In most cases, I "watermark" my final product and keep the final recording until the final payment is received.
      </p>

      <p>
        Regardless of your budget, if you are interested in building a relationship, I strongly encourage that you get
        in touch and we can discuss working something out.
      </p>

      <p>
        Remember, as my client, you are paying for a product as well as my service. I truly love this industry and
        insist upon a respectful working relationship.
      </p>
    </div>
  </div>
</div>

<style>
  .rates-content {
    text-align: left;
    line-height: 1.8;
    max-width: 100%;
    overflow-wrap: break-word;
    word-wrap: break-word;
    hyphens: auto;
  }

  .rates-content h3 {
    font-family: var(--heading-font);
    color: var(--title-bg-color);
    font-size: 1.8rem;
    margin-top: 2.5rem;
    margin-bottom: 1rem;
    line-height: 1.3;
  }

  .rates-content ul {
    list-style-type: disc;
    padding-left: 1.5rem;
    margin: 0 0 1.5rem 0;
    width: 100%;
  }

  .rates-content li {
    font-family: var(--body-font);
    font-style: italic;
    font-size: 1rem;
    margin-bottom: 0.75rem;
    padding-right: 1rem;
  }

  .rates-content p {
    font-family: var(--body-font);
    font-style: italic;
    font-size: 1rem;
    margin-bottom: 1.5rem;
    padding: 0 0.5rem;
  }

  .rates-content a {
    color: var(--accent-color);
    text-decoration: none;
    word-break: break-all;
  }

  .rates-content a:hover {
    text-decoration: underline;
  }

  @media (max-width: 768px) {
    .rates-content {
      padding: 0 0.5rem;
    }

    .rates-content h3 {
      font-size: 1.5rem;
      margin-top: 2rem;
    }

    .rates-content ul {
      padding-left: 1.25rem;
    }

    .rates-content li,
    .rates-content p {
      font-size: 0.95rem;
      line-height: 1.6;
    }
  }
</style>
