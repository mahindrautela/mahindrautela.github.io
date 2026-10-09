---
layout: home
title: Latent Evolution Models
description: "Latent evolution models for forward and inverse modeling, uncertainty quantification, and optimization of charged-particle beam dynamics."
permalink: /lem/
---

<section class="archive-hero section-tint">
  <div class="shell">
    <p class="section-kicker">Scientific machine learning</p>
    <h1>Latent evolution models</h1>
    <p>Forward and inverse modeling, uncertainty quantification, and tuning of charged-particle beam dynamics in particle accelerators.</p>
  </div>
</section>

<section class="research-archive section shell" markdown="1">

## Spatiotemporal learning of charged-particle beam dynamics (in particle accelerators)
The 6D phase space (x, y, z, p<sub>x</sub>, p<sub>y</sub>, p<sub>z</sub>) of charged-particle bunches evolves under the influence of electromagnetic fields along the accelerator. This can be viewed as a spatiotemporal dynamical system in which parameters such as RF-cavity amplitude and phase and magnet strength modulate the charged-particle beam.
1. In this [paper](https://www.nature.com/articles/s41598-024-68944-0), we propose a two-step unsupervised deep-learning framework called the *Conditional Latent Autoregressive Recurrent Model (CLARM)* for learning forward spatiotemporal dynamics.
   * The model can generate phase space at various accelerator modules by sampling and decoding the structured latent space representation.
   * The model also forecasts future states (downstream states) of charged particles from past states (upstream states). Learn more on the [project page](https://github.com/lanl/clarm).

<p align="center">
  <img src="/images/clarm_lansce.png" width="400" height="250" alt="CLARM latent evolution model for charged-particle beam dynamics" />
</p>

2. In this [paper](https://arxiv.org/abs/2408.07847), we use a reverse latent evolution model (CLARM is a special case of a broader LEM) to solve the *inverse problem* of predicting 6D phase-space projections across all upstream sections from downstream phase-space measurements.
   * The proposed model also captures the *aleatoric uncertainty* of the high-dimensional input data within the latent space.
   * The uncertainty is propagated through the temporal learner in the latent space to estimate bounds for all upstream predictions, demonstrating robustness to in-distribution variations in the input data.

3. In this [paper](https://arxiv.org/abs/2412.01748), we use a *classifier-pruned Bayesian optimizer* for efficient exploration within a *temporally structured latent space*.
   * CBOL-Tuner adaptively searches and filters the latent space for optimal solutions (i.e., RF settings for minimal beam loss in the accelerator).
   * CBOL-Tuner demonstrates superior performance in identifying multiple optimal settings and outperforms alternative global optimization methods.

<p align="center">
  <img src="/images/cbol.png" width="400" height="270" alt="CBOL-Tuner optimization workflow in a temporally structured latent space" />
</p>

</section>
