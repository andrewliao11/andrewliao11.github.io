---
layout: none
title: vlms_feedback
permalink: /draft_vlms_feedback/
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
        <source src="/assets/video/vlms_feedback/cropped_website_teaser_gif_vlm_feedback.mp4" type="video/mp4">
      </video>
      <h2 class="subtitle has-text-centered">
        <!--Can VLMs improve their responses by taking <i>self-generated</i> feedback? -->
        Can Feedback Enhance Semantic Grounding in Large Vision-Language Models?
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
            Enhancing semantic grounding abilities in Vision-Language Models (VLMs) often involves collecting domain-specific training data, refining the network architectures, or modi- fying the training recipes. In this work, we venture into an orthogonal direction and explore whether VLMs can improve their semantic grounding by "receiving" to feedback &#128172;, without requiring in-domain data, fine-tuning, or modifications to the network architectures. We systematically analyze this hypothesis using a feedback mechanism composed of a binary signal. We find that if prompted appropriately, VLMs can utilize feedback both in a single step and iteratively, showcasing the potential of feedback as an alternative technique to improve grounding in internet-scale VLMs. Furthermore, VLMs, like LLMs, struggle to self-correct errors out-of-the-box. However, we find that this issue can be mitigated via a binary verification mechanism. Finally, we explore the potential and limitations of amalgamating these findings and applying them iteratively to automatically enhance VLMs' grounding performance, showing grounding accuracy consistently improves using automated feedback across all models in all settings investigated. Overall, our iterative framework improves semantic grounding in VLMs by more than 15 accuracy points under noise-free feedback and up to 5 accuracy points under a simple automated binary verification mechanism &#128640;.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="hero is-light is-small" id="semi_interactive_demo">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column">
          <h2 class="title is-3">Give it a try! Provide your feedback to our VLM and see if it's doing well.</h2>
          <div class="columns is-centered">
            <div class="column content">
              <p>Here, you can interact with <a href="https://huggingface.co/liuhaotian/llava-v1.5-13b">LLaVA-1.5 13b model</a> by providing binary feedback.</p>
              <img src="/assets/img/vlms_feedback/demo_placeholder.png" />
              <p><small><sup>*</sup>All results are pre-generated.</small></p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="feedback_dynamics">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Use Prompt-based Feedback to Improve VLMs</h2>
        <div class="content">
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
            <p>We first study the foundamental questions (1) Can VLMs <font color="#ff0000">receive</font> prompt-based feedback? and (2) Can VLMs <font color="#ff0000">give</font> prompt-based feedback? We study these questions in the context of semantic grounding and investigate three open-sourced VLMs (LLaVA-1.5, ViP-LLaVA, and CogVLM) and one proprietary VLM (GPT-4V & SoM). Here, we summarize our findings and contributions</p>
            <div style="padding-left: 24px">
            <ol>
                <li><b>&#128172; VLMs can receive feedback to improve downstream semantic grounding</b>: Our study shows that VLMs improve &#128640; 4 to 12 accuracy points when recieving orale feedback that indicates the correctness of the prediction. When prompted over multiple rounds, VLMs improves by over 15 accuracy points &#128640;. This shows the potential of feedback as a means of improving grounding performance in VLMs.</li>
                <li><b>&#128483; VLMs can give binary feedback</b>: In line with the prior literature in LLMs, VLMs struggles to self-correction (Kim et al., 2023), but succeed in self-evaluation (Kadavath et al., 2022).  We show that VLMs can provide high-quality binary feedback through different visual prompts, <i>i.e.</i>, isolation or marking of objects.</li>
                <li><b>&#129302; Combining 1 and 2, VLMs benefit from automatic iterative feedback</b>: We formulate an iterative framework that improve semantic grounding in VLMs up to nearly 5 accuracy points.</li>
            </ol>
            </div>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="experiment">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Iterative Feedback Improves Semantic Grounding in VLMs</h2>
        <div class="content">
            We introduce an iterative loop of dialogue between a VLM agent and Verifier. At the first time step, the VLM agent obtain base predictions for every scene. We then prompt a verifier (the same VLM) to generate a binary feedback for every prediction. In the next time step, we provide this binary feedback to the VLM agent and ask it to re-generate predictions. We repeat these steps until Verifier agrees with the predictions. 
        </div>
        <div class="container is-centered">
          <video id="teaser" autoplay muted loop playsinline height="100%"><source src="/assets/video/vlms_feedback/website_framework_flow_gif.mp4" type="video/mp4">
        </video>
      </div>
        <h3 class="title is-4">&#128290; Quantitative Results</h3>
        <div class="content">
            We compare our approach, <i>VLM binary verification</i>, with <i>intrinsic self-correction</i> (Kim et al., 2023). We also compare with a noise-free version of our iterative approach, noise-free verification. The following table show the results on ADE20k<sup>*</sup>:<br><small><sup>*</sup>We use a subset of ADE20k validation images for evaluation.</small>
          <img src="/assets/img/vlms_feedback/ade_quantative_res.jpg" margin-left="auto" margin-right="auto"/>
          <p> We highlight the performance difference <i>w.r.t.</i> the performance of the base predictions and if the performances are below the performance of the base predictions, we use <font color="#ff0000">red-colored font.</font> </p>
        </div>
        <h3 class="title is-4">&#127912; Qualitative Results</h3>
        <div class="content">
          <img src="/assets/img/vlms_feedback/additional_qualitative_res_gpt4v_1.jpg" margin-left="auto" margin-right="auto"/>
        </div>
        <div class="content">
          <p> Here, we show an example using GPT-4V & SoM (Jianwei Yang et al., 2023) as the VLM. GPT-4V is able to identify what objects are in the image, but struggles to identify the mapping between numeric object IDs with objects. With self-generated feedback (from center to left), GPT-4V successfully corrects its own predictions. For more qualitative results, please refere to our paper. </p>
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