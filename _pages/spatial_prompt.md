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
          <div class="column has-text-centered" style="font-size: 2em; color: red; font-weight: bold;">EMNLP 2024</div>
          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="https://web3.arxiv.org/abs/2409.09788" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span>
              <!-- Code Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="https://github.com/andrewliao11/Q-Spatial-Bench-code" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                </a>
              </span>
              <!-- Data Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="https://huggingface.co/datasets/andrewliao11/Q-Spatial-Bench" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fa-solid fa-database"></i>
                  </span>
                  <span>Dataset</span>
                </a>
              </span>
              <span class="link-block">
                <a href="https://youtu.be/-eLdGq6JWiQ?si=yG2l_JKjb25SLwTm" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-youtube"></i>
                  </span>
                  <span>Video</span>
                </a>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="hero teaser">
  <div class="container is-max-desktop">
    <div style="text-align: center;">
      <img src="/assets/img/spatial_prompt/short_gif.gif" width="75%" margin-left="auto" margin-right="auto"/>
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



<section class="section" id="">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Why Quantitative Spatial Reasoning?</h2>
        <div class="content">
            <p>Spatial reasoning is essential for humans to interact with the world, such as determining if there is enough room on a desk for a backpack; if there is enough space to navigate through a room without hitting any obstacles; or if an object is placed sufficiently high enough to be inaccessible to a child.</p>
        </div>
        <div class="content">
            <h3 class="title is-4">Our contributions and findings</h3>
            <p>
            <div style="padding-left: 36px">
                <ol>
                    <li>We introduce <strong>Q-Spatial Bench</strong>, a benchmark that evaluates the quantitative spatial reasoning in large vision-language models.</li>
                    <li>Perhaps surprisingly, we find that GPT-4o outperforms other closed-source VLMs by a large margin.</li>
                    <li>We develop <strong>SpatialPrompt</strong>, a prompting technique that consistently improve quantitative spatial reasoning in VLMs.</li>
                </ol>
            </div>
            </p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Q-Spatial Bench</h2>
        <div class="content">
            <p><strong>Motivation:</strong> Current benchmarks primarily assess whether these models understand qualitative concepts like "left" versus "right" or "near" versus "far" from monocular images. However, recent studies have revealed that state-of-the-art VLMs struggle with quantitative spatial tasks. While measuring sizes or distances from monocular images is ill-posed, humans are surprisingly adept at mak- ing such estimations by relying on contextual clues.</p>
            <p><strong>Setup</strong> We explore quantitative spatial reasoning where a VLM is tasked to recognize quantitative spatial information of physical objects such as distances or sizes from a 2D image. In particular, we consider <i>direct</i> quantitative spatial reasoning, where a VLM predicts the quantitative spatial information <i>without</i> accessing any external tools or large models.</p>
            <p><strong>This work:</strong> In this paper, we introduce a new question answering corpora, Q-Spatial Bench, specifically designed to evaluate quantitative spatial reasoning in VLMs with high-precision. </p>
            <img src="/assets/img/spatial_prompt/dataset_stats.png" margin-left="auto" margin-right="auto"/>
        </div>
        <h2 class="title is-3">GPT-4o dominates in Q-Spatial Bench</h2>
        <div class="content">
            Prior works (Chen et al., 2024 and Cheng et al., 2024) suggest that state-of-the-art VLMs, e.g., GPT-4V, struggle in quantitative spatial reasoning. Perhaps surprisingly, we find the GPT-4o performs reasonably well in the proposed benchmark. Specifically, GPT-4o achieves more than 60 points in success rates in both splits of Q-Spatial Bench, while the second-best VLM gets no more than 30 points in success rates.
          <img src="/assets/img/spatial_prompt/gpt4o-is-good.png" margin-left="auto" margin-right="auto"/>
        </div>
        <h2 class="title is-3">GPT-4o dominates in Q-Spatial Bench</h2>
        <div class="content">
            Interestingly, we find that GPT-4o tends to use reference objects in its reasoning path and estimate the answer at the end. We, therefore, hypothesize that <i>Using reference objects for quantitative spatial reasoning leads to strong performances.</i>
            To validate our hypothesis, we collect the GPT-4o responses from both splits and use a logistic regression model for the analysis. For each response, we can derive four variables: (1) if the response is considered as a success or not (Y), (2) the source of data split (X1), (3) the ground truth distances (X2), and (4) if the response use any reference objects (X3). By using the success of each response as target, we fit a logistic regression model on them. We find that using reference objects in the responses increase the odds of the success variable by more than 250 percent in a statistically significant manner!
          <img src="/assets/img/spatial_prompt/gpt4o_responses.png" margin-left="auto" margin-right="auto"/>
        </div>
        <h2 class="title is-3">Spatial Prompt</h2>
        <div class="content">
            <p>Inspired by the above analysis, we develop a prompting technique to encourage VLM to perform quantitative spatial reasoning with referecen objects. We call this "SpatialPrompt".</p>
            <p>SpatialPrompt consistently improves all VLM testede in both splits of Q-Spatial Bench, improving Gemini-1.5-Pro by more than 40 points and GPT-4V by more than 30 points!</p>
            <img src="/assets/img/spatial_prompt/improvements.gif" margin-left="auto" margin-right="auto"/>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="BibTeX">
  <!-- Citation -->
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@inproceedings{
liaos2024reasoning,
title={Reasoning Paths with Reference Objects Elicit Quantitative Spatial Reasoning in Large Vision-Language Models},
author={Yuan-Hong Liao and Rafid Mahmood and Sanja Fidler and David Acuna},
booktitle={The 2024 Conference on Empirical Methods in Natural Language Processing},
year={2024},
url={https://arxiv.org/abs/2409.09788},
}</code></pre>
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
