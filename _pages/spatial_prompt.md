---
layout: none
title: spatial_prompt
permalink: /spatial_prompt/
nav: false

---

<head>
  <meta charset="utf-8">
  <title>Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models</title>
  <meta name="description"
    content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models">
  <meta name="keywords" content="vision-language models, spatial reasoning, prompt engineering, vlm benchmark">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta property="og:title" content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models">
  <meta property="og:type" content="website">
  <meta property="og:site_name"
    content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models">
  <meta property="og:image"
    content="" />
  <!-- todo -->
  <meta property="og:image:type" content="image/png" />
  <meta property="og:image:width" content="1082" />
  <meta property="og:image:height" content="639" />
  <meta property="og:url" content="" />
  <meta property="og:description" content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models" />
  <meta name="twitter:title"
    content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models" />
  <meta name="twitter:description" content="Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models" />
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
          <h1 class="title is-1 publication-title">Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models</h1>
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
                <a href="https://github.com/andrewliao11/spatial_prompt" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                </a>
              </span>
              <!-- Data Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fa-solid fa-database"></i>
                  </span>
                  <span>Dataset</span>
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


<section class="section" id="abstract">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          <p>
Despite recent advances demonstrating vision- language models’ (VLMs) abilities to describe complex relationships in images using natural language, their capability to quantitatively reason about object sizes and distances remains underexplored. In this work, we introduce a manually annotated benchmark, Q-Spatial Bench, with 271 questions across five categories designed for quantitative spatial reasoning and systematically investigate the performance of state-of-the-art VLMs on this task. Our analysis reveals that reasoning about distances between objects is particularly challenging for SoTA VLMs; however, some VLMs significantly outperform others, with an over 40-point gap between the two best performing models. We also make the surprising observation that the success rate of the top-performing VLM increases by 19 points when a reasoning path using a reference object emerges naturally in the response. Inspired by this observation, we develop a zero-shot prompting technique, SpatialPrompt, that encourages VLMs to answer quantitative spatial questions using reference objects as visual cues. By instructing VLMs to use reference objects in their reasoning paths via SpatialPrompt, Gemini 1.5 Pro, Gemini 1.5 Flash, and GPT-4V improve their success rates by over 40, 20, and 30 points, respectively. We emphasize that these significant improvements are obtained without needing more data, model architectural modifications, or fine-tuning.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>



<section class="section" id="feedback_dynamics">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Do all VLMs struggle at quantitative spatial reasoning?</h2>
        <div class="content">
            <p>No! Prior works (Chen et al., 2024 and Cheng et al., 2024) show that state-of-the-art VLMs, such as GPT-4V, struggle at quantitative spatial reasoning. However, we find that the latest GPT-4o demonstrates a significant jump from GPT-4V with a 41 success rate improvement.</p>
            <p>Despite VLMs’ strong visual-language understanding abilities, <i>fine-grained visual grounding</i> remains a challenge. This work investigates how <font color="#ff0000">prompt-based feedback</font> can improve semantic grounding in VLMs. This enjoys two main advantages: 
            <div style="padding-left: 36px">
                <ol>
                    <li>&#128293; Requiring no additional training</li>
                    <li>&#128293; Unleashing services relying on API-based VLMs for their downstream applications</li>
                </ol>
            </div>
            </p>
        </div>
        <div class="content">
            <h3 class="title is-4">Feedback Dynamics in VLMs</h3>
        </div>
      </div>
    </div>
  </div>
</section>



<section class="section" id="BibTeX">
  <!-- Citation -->
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>[bibtex here]</code></pre>
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
