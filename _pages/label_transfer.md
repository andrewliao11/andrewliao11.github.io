---
layout: none
title: label_transfer
permalink: /label_transfer/
nav: false

---

<head>
  <meta charset="utf-8">
  <title>Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets</title>
  <meta name="description"
    content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets">
  <meta name="keywords" content="labe transfer, data-centric, object detection, domain adaptation">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta property="og:title" content="V">
  <meta property="og:type" content="website">
  <meta property="og:site_name"
    content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets">
  <meta property="og:image"
    content="" />
  <!-- todo -->
  <meta property="og:image:type" content="image/png" />
  <meta property="og:image:width" content="1082" />
  <meta property="og:image:height" content="639" />
  <meta property="og:url" content="" />
  <meta property="og:description" content="Project page for Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
  <meta name="twitter:title"
    content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
  <meta name="twitter:description" content="Project page for Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
  <meta name="twitter:image"
    content="" />

  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-slider.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/fontawesome.all.min.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/index.css">
  <link rel="icon" href="/assets/external_pages/label_transfer/static/images/vlmaps_icon.svg">

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
          <h1 class="title is-1 publication-title">Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets</h1>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://andrewliao11.github.io">Yuan-Hong Liao</a><sup>2</sup>,</span>
            <span class="author-block">
              <a href="http://www.cs.toronto.edu/~davidj/">David Acuna</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://rafidrm.github.io">Rafid Mahmood</a><sup>1, 3</sup>,</span>
            <span class="author-block">
              <a href="https://www.cs.toronto.edu/~jlucas/">James Lucas</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://virajprabhu.github.io">Viraj Prabhu</a><sup>4</sup>,</span>
            <span class="author-block">
              <a href="https://www.cs.utoronto.ca/~fidler/">Sanja Fidler</a><sup>1, 2</sup></span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>NVIDIA,</span>
            <span class="author-block"><sup>2</sup>University of Toronto, Vector Institute, </span>
            <span class="author-block"><sup>3</sup>University of Ottawa, </span>
            <span class="author-block"><sup>4</sup>Georgia Institute of Technology</span>
          </div>
          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              <span class="link-block"> <!-- todo -->
                <a href="https://openreview.net/forum?id=ChHx5ORqF0" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
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
            In object detection, varying annotation protocols across datasets can result in <i>annotation mismatches</i>, leading to inconsistent class labels and bounding regions. Addressing these mismatches typically involves manually identifying common trends and fixing the corresponding bounding boxes and class labels. To alleviate this laborious process, we introduce the label transfer problem in object detection. Here, the goal is to transfer bounding boxes from one or more source datasets to match the annotation style of a target dataset. We propose a data-centric approach, Label-Guided Pseudo-Labeling (LGPL), that improves downstream detectors in a manner agnostic to the detector learning algorithms and model architectures. Validating across four object detection scenarios, defined over seven different datasets and three different architectures, we show that transferring labels for a target task via LGPL <i>consistently improves</i> the downstream detection in every setting, on average by 1.88 mAP and 2.65 AP^{75}. Most importantly, we find that when training with multiple labeled datasets, carefully addressing annotation mismatches with LGPL alone can improve downstream object detection better than off-the-shelf supervised domain adaptation techniques that align instance features.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="annotation_mismatches">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">What are annotation mismatches</h2>
        <div class="content has-text-justified has-text-centered">
          <h3 class="title is-4">Not all bicycles are labled in the same way</h3>
            <img src="" /> <!-- a zoom-in image of bicycles mismatches between datasets -->
            <p> Show some interesting bicycle images</p>
          <h3 class="title is-4">Taxonomy of annotation mismatches</h3>
            <img src="" /> <!-- More examples here -->
            <p> We categorize annotations mismatches into four common types: ...</p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="approach">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Approach</h2>
        <div class="content has-text-justified has-text-centered">
          <h3 class="title is-4">A data-centric approach: Label Transfer</h3>
            <p> Define what label transfer is</p>
          <h3 class="title is-4">Label-guided Pseudo-Labeling (LGPL)</h3>
            <img src="" /> <!-- A GIF can help a lot -->
            <p> A simple label transfer model is secretly in your two-stage object detector.</p>
            <p> Training</p>
            <p> Inference</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="experiment">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Experiments</h2>
        <div class="content has-text-justified has-text-centered">
          <p> Briefly describe the four scenarios we have in the paper</p>
          <h3 class="title is-4">LGPL consistently improves downstream detectors</h3>
            <img src="" /> <!-- a condensed version of table 1 and 2 -->
            <p> What does this imply? Be brief and highlight with bold font</p>
          <h3 class="title is-4">Label transfer outperform image transfer</h3>
            <img src="" /> <!-- figure 4 -->
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
    <pre><code>@inproceedings{
liao2024translating,
title={Translating Labels to Solve Annotation Mismatches Across Object Detection Datasets},
author={Yuan-Hong Liao and David Acuna and Rafid Mahmood and James Lucas and Viraj Uday Prabhu and Sanja Fidler},
booktitle={The Twelfth International Conference on Learning Representations},
year={2024},
url={https://openreview.net/forum?id=ChHx5ORqF0}
} </code></pre>
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