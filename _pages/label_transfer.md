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
  <meta property="og:title" content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets">
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
  <meta property="og:description" content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
  <meta name="twitter:title"
    content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
  <meta name="twitter:description" content="Transferring Labels to Solve Annotation Mismatches Across Object Detection Datasets" />
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
          <div class="column has-text-centered" style="font-size: 2em; color: red; font-weight: bold;">ICLR 2024</div>
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
              <span class="link-block">
                <a href="https://iclr.cc/virtual/2024/poster/19161" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-youtube"></i>
                  </span>
                  <span>Video</span>
                </a>
              </span>
              <span class="link-block"> <!-- todo -->
                <a href="/assets/img/label_transfer/poster_best_reduced.pdf" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Poster</span>
                </a>
              </span>
              <span class="link-block"> <!-- todo -->
                <a href="https://iclr.cc/media/iclr-2024/Slides/19161.pdf" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Slides</span>
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
    <div class="hero-body">
      <!--<video id="teaser" autoplay muted loop playsinline height="100%">
        <source src="static/videos/PR2LAnimation.mp4" type="video/mp4">
      </video> -->
      <div style="text-align: center;">
        <img src="/assets/img/label_transfer/teaser.png" width="75%" margin-left="auto" margin-right="auto"/>
      </div>
      <h2 class="subtitle has-text-centered">
        Can you find any cyclist/bicycle label errors across the six images?<br>
        <small>In fact, they are all correct! From left to right columns, they are Cityscapes, Waymo, nuImages, respectively.</small>
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
        <h2 class="title is-3">Annotation mismatches</h2>
        <div class="content has-text-justified has-text-centered">
          <h3 class="title is-4">What are annotation mismatches?</h3>
            <p>Annotation mismatches stem from <strong>diﬀerences in annotation protocols</strong>, including class taxonomies, instructions, and label post-processing, etc. <br>
            For example, in the figure below, Mapillary Vistas Dataset (MVD) annotates cyclists as ‘riders’, while Waymo Open Dataset (Waymo) combines riders and bicycles into the ‘cyclist’ class. On the other hand, nuImages annotates bikes on sidewalks, but Waymo excludes these per the annotation instructions. In addition to the ontological mismatches, discrepancies of annotation instructions, human-machine misalignment, and cross-modality labels result in unique annotation mismatches.</p>
            <img src="/assets/img/label_transfer/annotation_mismatch_example.png" width="100%" margin-left="auto" margin-right="auto"/>
          <h3 class="title is-4">Why does it matter?</h3>
            <p>Training on datasets with annotation mismatches, such as combining nuImages and Waymo, can introduce unwanted biases and confuse models, like causing detectors to misidentify bikes on sidewalks. We propose <strong>a data-centric approach</strong> to resolve these mismatches across datasets, enhancing the performance of downstream detectors in a model-agnostic manner.</p>
        </div>
      </div>
    </div>
  </div>
</section>



<section class="section" id="approach">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Label Transfer</h2>
        <div class="content has-text-justified has-text-centered">
          <p>In this work, we propose the "Label Transfer" problem, where a label transfer model needs to adjust the source labels such that the tranferred labels follow the annotation protocol in the target dataset. We evaluate the effectiveness by the performances of the induced downstream detectors.</p>
          <p><strong>Main challenge</strong>: there is no paired labels on the same image in the datasets.</p>
          <h3 class="title is-4">Label-Guided Pseudo-Labeling (LGPL)</h3>
            <p>To mitigate annotations mismatches, we may use a model trained on the target data to generate pseudo-labels on the source images (Arazo et al., 2019; Lee, 2013), but this discards the existing source labels. On the other hand, statistical normalization (Wang et al., 2020) aligns boxes statistics but ignores the image content. Label-guided pseduo-lableing aims to fully leverate all available information for the label transfer problem</p>
            <p>LGPL is inspired by identifying that the strategy used in two-stage object detectors. In short, we trained the RPN network on the source datasets and apply source-trained RPN to produce source-like proposals on the target images. Finally, we train the RoI head to transfer the source-like proposals on the target images to the target labels. All the components can be trained end-to-end.</p>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="section" id="experiment">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Experimental results</h2>
        <div class="content has-text-justified has-text-centered">
          <p>We experimented across 4 transferring scenarios and 3 detector architecures. We adopt 5 baseline apporaches to the label transfer problem to showcase the effectiveness of LGPL. Please see the paper for more details</p>
          <div style="text-align: center;">
          <img src="/assets/img/label_transfer/results.png" width="80%" margin-left="auto" margin-right="auto"/>
          </div>
          <p>Here are our findings</p>
          <div style="padding-left: 24px">
          <ol>
              <li>LGPL outperforms all other baseline methods for every architecture.</li>
              <li>Transferring labels leads to higher-quality object detectors.</li>
              <li>LGPL outperforms off-the-shelf supervised domain adaptation.</li>
              <li>Off-the-shelf segmentation foundation models fall short in label transfer.</li>
          </ol>
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