---
layout: none
title: LongPerceptualThoughts Distilling System-2 Reasoning for System-1 Perception
permalink: /LongPerceptualThoughts/
nav: false

---

<head>
  <meta charset="utf-8">
  <title>LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception</title>
  <meta name="description"
    content="LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception">
  <meta name="keywords" content="vision-language models, visual reasoning, system-2 reasoning">
  <meta name="viewport" content="width=device-width, initial-scale=1">

   <!-- Open Graph Metadata -->
  <meta property="og:title" content="LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception">
  <meta property="og:type" content="website">
  <meta property="og:site_name"
    content="LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception">
  <meta property="og:image"
    content="" />
  <meta property="og:image:type" content="image/png" />
  <meta property="og:image:width" content="1082" />
  <meta property="og:image:height" content="639" />
  <meta property="og:url" content="" />
  <meta property="og:description" content="LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception" />
  <meta name="twitter:title" content="LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception" />
  <meta name="twitter:description" content="We study how to leverage system-2 reasoning to solve perception tasks and introduce LongPerceptualThoughts, a new synthetic dataset of 30k long chain-of-thought traces for vision tasks." />
  <meta name="twitter:image"
    content="/assets/img/long_perceptual_thoughts/data_pipeline.gif" />

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Crimson+Pro:ital,wght@0,200..900;1,200..900&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

  <!-- CSS -->
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/bulma-slider.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/fontawesome.all.min.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="/assets/external_pages/label_transfer/static/css/index.css">
  <link rel="icon" href="/assets/img/logo.jpg">

  <!-- JavaScript -->
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script defer src="/assets/external_pages/label_transfer/static/js/fontawesome.all.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/bulma-carousel.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/bulma-slider.min.js"></script>
  <script src="/assets/external_pages/label_transfer/static/js/index.js"></script>
  <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
  <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

  <!-- Custom Font Override -->
  <style>
    body, .title, .author-block {
      font-family: 'Crimson Pro', serif !important;
    }
    /* Podcast Section Styling */
    .podcast-section {
      background-color: #f0f8ff;
      border-radius: 8px;
      border-left: 5px solid #3273dc;
    }
    
    .podcast-title {
      color: #3273dc;
    }
    
    .podcast-player {
      margin-top: 1rem;
      width: 100%;
      max-width: 800px;
    }
    
  </style>
</head>


<section class="hero" >
  <div class="hero-body" style="padding-top: 2rem; padding-bottom: 2rem;">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-1 publication-title">LongPerceptualThoughts: Distilling System-2 Reasoning for System-1 Perception</h1>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://andrewliao11.github.io">Yuan-Hong Liao</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://selflein.github.io">Sven Elflein</a><sup>1, 2</sup>,</span>
            <span class="author-block">
              <a href="https://arking1995.github.io">Liu He</a><sup>3</sup>,</span>
            <span class="author-block">
              <a href="https://dvl.in.tum.de/team/lealtaixe/">Laura Leal-Taixe ́</a><sup>2</sup>,</span>
            <span class="author-block">
              <a href="https://yejinc.github.io">Yejin Choi</a><sup>2</sup>,</span>
            <span class="author-block">
              <a href="https://www.cs.utoronto.ca/~fidler/">Sanja Fidler</a><sup>1, 2</sup>,</span>
            <span class="author-block">
              <a href="http://www.cs.toronto.edu/~davidj/">David Acuna</a><sup>2</sup></span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>University of Toronto, Vector Institute, </span>
            <span class="author-block"><sup>2</sup>NVIDIA,</span>
            <span class="author-block"><sup>3</sup>Purdue University</span>
          </div>
          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              <span class="link-block"> 
                <a href="LINK" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span>
              <!-- Code Link. -->
              <span class="link-block"> 
                <a href="https://github.com/andrewliao11/LongPerceptualThoughts" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                </a>
              </span>
              <!-- Dataset Link. -->
              <span class="link-block"> 
                <a href="https://huggingface.co/datasets/andrewliao11/LongPerceptualThought" class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                    <i class="fas fa-database"></i>
                  </span>
                  <span>Dataset</span>
                </a>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Podcast Section -->
<section class="section" style="padding-top: 0rem; padding-bottom: 3rem;">
  <div class="container is-max-desktop">
    <div class="columns is-centered is-mobile">
      <div class="column is-four-fifths podcast-section" style="max-width: 70%; padding: 10px 30px 15px;">
        <h2 class="title is-4 podcast-title">
          <i class="fas fa-podcast"></i> Notebook LM Summary
        </h2>
        <div class="content">
          <p>Commuting? Listen to our paper's key insights in just minutes!</p>
          <div class="podcast-player">
            <audio controls style="width: 100%;">
              <source src="/assets/audio/long_perceptual_thoughts/from_notebook_lm.wav" type="audio/wav">
              Your browser does not support the audio element.
            </audio>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="summary">
<div class="container is-max-desktop">
    <div class="columns is-centered is-mobile">
      <div class="column is-four-fifths" style="max-width: 70%; background-color: #f5f5f5; padding: 30px 30px 39px;">
        <div class="title is-4" style="margin-bottom: 0.5em">🔍 Project summary:</div>
        <div class="content has-text-justified">
          <p>
            We study how to leverage system-2 reasoning to solve perception tasks, the kind of tasks VLMs typically handle with fast, shallow (system-1) thinking. Here's what we found:
          </p>
          <ul>
            <li>
              With <i>LongPerceptualThoughts</i>, VLMs can perform system-2 reasoning on perceptual tasks <b>after simple supervised fine-tuning</b>.
            </li>
            <li>
              Surprisingly, despite being tuned only on visual tasks, these fine-tuned VLMs <b>generalize well to challenging text-only reasoning benchmarks like MMLU-Pro!</b>
            </li>
          </ul>
        </div>
        <div class="title is-4" style="margin-bottom: 0.5em">🎯 So, what’s the secret sauce here?</div>
        <div class="content has-text-justified">
          <p>
            We introduce LongPerceptualThoughts, a synthetic dataset of 30K long chain-of-thought (CoT) traces for vision tasks. We synthesize these long CoTs with <b>a novel three-stage data synthesis framework</b> that effectively incorporates key cognitive behaviors such as backtracking, verification, subgoal setting, etc., in the long CoTs.
          </p>
          <p>
            Overall, by fine-tuning on LongPerceptualThoughts,we improve Qwen2.5-VL-7B on 5 vision-centric benchmarksby by <b>an average of 3.4 points</b>. In particular, we improve V* bench by 11.8 points. We even find that the fine-tuned Qwen2.5-VL improves <b>out-of-distribution MMLU-Pro</b> by more than 2 points!
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="introduction">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Introduction</h2>
        <div class="content">
            <p>Despite the rapid progress in reasoning-focused models like OpenAI’s o1 and DeepSeek’s R1, most advances have focused on math and code domains. But what about perception -- tasks like object recognition, scene understanding, or spatial reasoning, where vision-language models (VLMs) typically rely on fast, shallow reasoning? 
            </p>
            <p>
            This work asks: <b>Can we equip VLMs with system-2 reasoning to improve performance on vision-centric tasks?</b> And our answer is Yes! and with only 500 images! 
            </p>
        </div>
        <div class="table-container" align="center">
            <table class="table is-striped is-hoverable">
                <thead>
                <tr>
                    <th class="has-background-grey-lighter">Method</th>
                    <th class="has-background-grey-lighter">Avg</th>
                    <th class="has-background-grey-lighter">CV-Bench</th>
                    <th class="has-background-grey-lighter">V* Bench</th>
                    <th class="has-background-grey-lighter">MMVP</th>
                    <th class="has-background-grey-lighter">MMStar-V</th>
                    <th class="has-background-grey-lighter">MME-RW-V</th>
                </tr>
                </thead>
                <tbody>
                <tr>
                    <th>Qwen2.5-VL-7B-Instruct</th>
                    <td>58.47</td>
                    <td>74.74</td>
                    <td>48.51</td>
                    <td>73.67</td>
                    <td>63.73</td>
                    <td>31.68</td>
                </tr>
                <tr>
                    <th>+ CoT</th>
                    <td>59.18</td>
                    <td>75.42</td>
                    <td>55.08</td>
                    <td>70.60</td>
                    <td>62.40</td>
                    <td>32.40</td>
                </tr>
                <tr>
                    <th class="has-background-info-light"><strong>+ LongPerceptualThoughts (SFT)</strong></th>
                    <td class="has-background-info-light"><strong>59.90</strong></td>
                    <td class="has-background-info-light">76.05</td>
                    <td class="has-background-info-light">60.53</td>
                    <td class="has-background-info-light">70.00</td>
                    <td class="has-background-info-light">60.67</td>
                    <td class="has-background-info-light">32.25</td>
                </tr>
                <tr>
                    <th class="has-background-info-light"><strong>+ LongPerceptualThoughts (SFT + DPO)</strong></th>
                    <td class="has-background-info-light"><strong>61.87</strong></td>
                    <td class="has-background-info-light"><strong>76.61</strong></td>
                    <td class="has-background-info-light"><strong>60.31</strong></td>
                    <td class="has-background-info-light"><strong>75.00</strong></td>
                    <td class="has-background-info-light"><strong>64.00</strong></td>
                    <td class="has-background-info-light"><strong>33.45</strong></td>
                </tr>
                </tbody>
            </table>
          </div>
          <div class="content">
            <div class="content has-text-centered mt-2 mb-4">
              <details class="disclosure-widget">
                <summary>For more results, please unfold to see expanded tables</summary>
                <!-- The detailed results table goes inside the details element -->
                <div id="detailed-results-container">
                  <h4 class="subtitle is-5 mt-4">Comparison with other multimodal reasoning datasets.</h4>
                    <div class="table-container" align="center">
                    <table class="table is-striped is-hoverable">
                      <thead>
                      <tr>
                          <th class="has-background-grey-lighter">Method</th>
                          <th class="has-background-grey-lighter">Avg</th>
                          <th class="has-background-grey-lighter">CV-Bench</th>
                          <th class="has-background-grey-lighter">V* Bench</th>
                          <th class="has-background-grey-lighter">MMVP</th>
                          <th class="has-background-grey-lighter">MMStar-V</th>
                          <th class="has-background-grey-lighter">MME-RW-V</th>
                      </tr>
                      </thead>
                      <tbody>
                      <tr>
                          <th>Qwen2.5-VL-7B-Instruct</th>
                          <td>58.47</td>
                          <td>74.74</td>
                          <td>48.51</td>
                          <td>73.67</td>
                          <td>63.73</td>
                          <td>31.68</td>
                      </tr>
                      <tr>
                          <th>+ CoT</th>
                          <td>59.18</td>
                          <td>75.42</td>
                          <td>55.08</td>
                          <td>70.60</td>
                          <td>62.40</td>
                          <td>32.40</td>
                      </tr>
                      <tr>
                          <th>+ VLAA-thinking <small>(Chen el al., 2025)</small></th>
                          <td>42.32</td>
                          <td>68.50</td>
                          <td>53.53</td>
                          <td>66.67</td>
                          <td>0.53</td>
                          <td>22.38</td>
                      </tr>
                      <tr>
                          <th>+ Virgo <small>(Du el al., 2025)</small></th>
                          <td>50.87</td>
                          <td>67.22</td>
                          <td>44.14</td>
                          <td>57.67</td>
                          <td>57.6</td>
                          <td>27.71</td>
                      </tr>
                      <tr>
                          <th class="has-background-info-light"><strong>+ LongPerceptualThoughts (SFT)</strong></th>
                          <td class="has-background-info-light"><strong>59.90</strong></td>
                          <td class="has-background-info-light">76.05</td>
                          <td class="has-background-info-light">60.53</td>
                          <td class="has-background-info-light">70.00</td>
                          <td class="has-background-info-light">60.67</td>
                          <td class="has-background-info-light">32.25</td>
                      </tr>
                      <tr>
                          <th class="has-background-info-light"><strong>+ LongPerceptualThoughts (SFT + DPO)</strong></th>
                          <td class="has-background-info-light"><strong>61.87</strong></td>
                          <td class="has-background-info-light"><strong>76.61</strong></td>
                          <td class="has-background-info-light"><strong>60.31</strong></td>
                          <td class="has-background-info-light"><strong>75.00</strong></td>
                          <td class="has-background-info-light"><strong>64.00</strong></td>
                          <td class="has-background-info-light"><strong>33.45</strong></td>
                      </tr>
                      </tbody>
                  </table>
                  </div>
                </div>
              </details>
            </div>
          </div>
      </div>
    </div>
  </div>
</section>  

<section class="section" id="approach">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Data Synthesis Framework: Ask, Think, and Think Harder</h2>
        <div class="content has-text-justified has-text-centered">
          <p>
            We propose a scalable, three-stage framework to synthesize long CoTs from <b>images and dense captions</b>:
          </p>
          <div class="container">
            <div class="columns is-centered">
                <div class="column is-narrow has-text-centered">
                <img src="/assets/img/long_perceptual_thoughts/data_pipeline.gif" alt="Data Pipeline" style="width: 70%;" />
                </div>
            </div>
            </div>
          <p>
            <ul>
              <li>
                <b>Stage 1 – Ask using an LLM:</b> We start by converting dense image descriptions into <b>multiple-choice questions</b> using GPT-4o-mini. These questions are designed to be <b>grounded</b>, <b>diverse</b>, and <b>verifiable</b>, ensuring the model has a clear visual task to reason about. 
              </li>
              <li>
                <b>Stage 2 – Think like a VLM:</b> Next, we use a <b>Qwen2.5-VL-7B-Instruct</b> to generate a <b>simple chain-of-thought (CoT)</b>. These are short, direct reasoning steps that are within the VLM’s comfort zone, providing a natural foundation to build deeper thoughts from.
              </li>
              <li>
                <b>Stage 3 – Think harder like a Reasoning VLM:</b> Finally, we hand over the image, question, and simple CoT to a <b>powerful reasoning LLM</b> (e.g., DeepSeek-R1-Distill). With a gentle nudge, like inserting "Wait," before the reasoning begins, we prompt the model to <b>reflect, verify, and revise</b> its thinking. The result? A rich, multi-step <b>long CoT</b> that mimics system-2 behavior: setting subgoals, checking assumptions, and even backtracking if needed.
              </li>
            </ul>
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="analysis">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Analysis: More Thoughtful Chains, Not Just Longer Ones</h2>
        <!-- Side-by-side figures -->
        <div class="columns is-centered">
          <div class="column has-text-centered">
            <figure>
              <img src="/assets/img/long_perceptual_thoughts/seq_len_change.pdf" alt="Length of CoTs" style="max-width: 100%;">
              <figcaption style="font-size: 0.9rem;">Token-length distribution of CoTs.</figcaption>
            </figure>
          </div>
          <div class="column has-text-centered">
            <figure>
              <img src="/assets/img/long_perceptual_thoughts/cognitive_analysis.pdf" alt="Cognitive Behaviors in CoTs" style="max-width: 100%;">
              <figcaption style="font-size: 0.9rem;">Frequency of cognitive behaviors in CoTs.</figcaption>
            </figure>
          </div>
        </div>
        <!-- Bullet points describing each figure -->
        <div class="content has-text-justified">
          <ul>
            <li>
              <b>CoT Lengths (left figure):</b> CoTs in LongPerceptualThoughts are longer on average as compared to CoT produced by popular VLMs.
            </li>
            <li>
              <b>Cognitive Behaviors (right figure):</b> CoTs in LongPerceptualThoughts also demonstrate diverse behaviors in structure. Unlike flat responses from baseline VLMs, our CoTs include intermediate steps and self-reflection. More specifically, our CoTs in LongPerceptualThoughts demonstrate significantly higher rates of subgoal setting, backtracking, and verification compared to VLMs like Qwen2.5-VL CoTs. 
              The CoTs in LongPerceptualThoughts are more similar to those generated by Gemini Flash Thinking, these structured behaviors are key indicators of system-2 reasoning, and are rarely observed in existing vision-language CoT datasets.
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="takeaways">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Takeaways</h2>
        <div class="content has-text-justified">
          <ol>
            <li>
              <b>🧠 Synthesizing long, rich reasoning data powers perception.</b><br>
              With just 500 images, we generate 30K chain-of-thought traces that teach vision-language models to reflect, verify, and revise. These cognitive patterns—rare in standard datasets—boost visual reasoning across benchmarks.
            </li>
            <li>
              <b>🥷 Just SFT. Nothing fancy.</b><br>
              No new architectures. No reinforcement learning from scratch. Just supervised fine-tuning on LongPerceptualThoughts leads to strong gains on vision-centric tasks. More surprisingly, it even improves performance on a text-only reasoning benchmark (MMLU-Pro). See more details in our paper!
            </li>
          </ol>
          <p><i>Richer thinking leads to better seeing—without needing more data or bigger models.</i></p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="BibTeX">
  <!-- Citation -->
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>
</code></pre>
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
