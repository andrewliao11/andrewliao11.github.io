---
layout: none
title: vlms_feedback
permalink: /vlms_feedback/
nav: false

---

<head>
  <meta charset="utf-8">
  <title>Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?</title>
  <meta name="description"
    content="Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?">
  <meta name="keywords" content="vision-language models, visual grounding, prompt engineering, feedback">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta property="og:title" content="Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?">
  <meta property="og:type" content="website">
  <meta property="og:site_name"
    content="Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?">
  <meta property="og:image"
    content="" />
  <!-- todo -->
  <meta property="og:image:type" content="image/png" />
  <meta property="og:image:width" content="1082" />
  <meta property="og:image:height" content="639" />
  <meta property="og:url" content="" />
  <meta property="og:description" content="Project page for Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?" />
  <meta name="twitter:title"
    content="Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?" />
  <meta name="twitter:description" content="Project page for Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?" />
  <meta name="twitter:image"
    content="" />

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-slider.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/fontawesome.all.min.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/index.css">
  <link rel="icon" href="/assets/img/logo.jpg">

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script defer src="/assets/external_pages/label_transfer/static/js/fontawesome.all.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/bulma-carousel.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/bulma-slider.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/index.js"></script>
</head>


<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-1 publication-title">Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?</h1>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://andrewliao11.github.io">Yuan-Hong Liao</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://rafidrm.github.io">Rafid Mahmood</a><sup>2, 3</sup>,</span>
            <span class="author-block">
              <a href="https://www.cs.utoronto.ca/~fidler/">Sanja Fidler</a><sup>1, 2</sup>,</span>
            <span class="author-block">
              <a href="http://www.cs.toronto.edu/~davidj/">David Acuna</a><sup>2</sup></span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>University of Toronto, Vector Institute, </span>
            <span class="author-block"><sup>2</sup>NVIDIA,</span>
            <span class="author-block"><sup>3</sup>University of Ottawa</span>
          </div>
          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span>
              <!-- Code Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                </a>
              </span>
              <!-- Video Link. 
              <span class="link-block">
                <a href="" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-youtube"></i>
                  </span>
                  <span>Video</span>
                </a>
              </span> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <video id="teaser" autoplay muted loop playsinline height="100%">
        <source src="static/videos/PR2LAnimation.mp4" type="video/mp4">
      </video>
      <h2 class="subtitle has-text-centered">
        TODO: caption for the GIF
      </h2>
    </div>
  </div>
</section>

<section class="section" id="abstract">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
            Enhancing semantic grounding abilities in Vision-Language Models (VLMs) often involves collecting domain-specific training data, refining the network architectures, or modi- fying the training recipes. In this work, we venture into an orthogonal direction and explore whether VLMs can improve their semantic grounding by "listening" to feedback, without requiring in-domain data, fine-tuning, or modifications to the network architectures. We systematically analyze this hypothesis using a feedback mechanism composed of a binary signal. We find that if prompted appropriately, VLMs can listen to feedback both in a single step and iteratively, showcasing the potential of feedback as an alternative technique to improve grounding in internet-scale VLMs. Furthermore, VLMs, like LLMs, struggle to self-correct errors out-of-the-box. However, we find that this issue can be mitigated via a binary verification mechanism. Finally, we explore the potential and limitations of amalgamating these findings and applying them iteratively to automatically enhance VLMs' grounding performance, showing grounding accuracy consistently improves using automated feedback across all models in all settings investigated. Overall, our iterative framework improves semantic grounding in VLMs by more than 15 accuracy points under noise-free feedback and up to 5 accuracy points under a simple automated binary verification mechanism.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="semi_interactive_demo">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Select an image and provide binary feedback</h2>
      </div>
    </div>
  </div>
</section>


<section class="section" id="feedback_dynamics">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Do VLMs receive and give feedback?</h2>
        We study this question by proposing four questions and systematically investigate how to approach it.
        <div class="content has-text-justified has-text-centered">
          <h3 class="title is-4">Experimental findings</h3>
            <p> Briefly show the takeaway</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="experiment">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Towards Iterative Self-Generated Feedback</h2>
        <div class="content has-text-justified has-text-centered">
          <p> Briefly describe the four scenarios we have in the paper</p>
          <h3 class="title is-4">Self-generated feedback is useful when coupled with explicit verifier and visual prompts techniques</h3>
            <img src="" /> <!-- a condensed version of table 1 and 2 -->
            <p> What does this imply? Be brief and highlight with bold font</p>
          <h3 class="title is-4">Qualitative results</h3>
            <img src="" /> <!-- show with lots of examples (side-by-side comparison) -->
        </div>
      </div>
    </div>
  </div>
</section>
  

<section class="section" id="BibTeX">
  <!-- Citation -->
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>to fill</code></pre>
  </div>
</section>

<section>
  <!-- Shout out to nerfies -->
  <div class="container is-max-desktop content">
    <footer class="footer">
      <div class="content">
        <p> Website borrowed from <a href="https://github.com/nerfies/nerfies.github.io">NeRFies</a> under a <a
            href="https://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0
            International</a>
        </p>
      </div>
    </footer> 
  </div>
</section>