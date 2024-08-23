---
layout: archive
title: ""
permalink: /research/
author_profile: true
---

## <ins>Research projects</ins>
## Charged particle beam dynamics in particle accelerators
* 6D phase space(x,y,x,px,py,pz) of charged particle bunches evolves under the influence of EM fields along the accelerator. The problem can be thought of as a spatiotemporal dynamical sytem, where the system parameters (like amplitude, phase of RF cavity, magnet strenth, etc.) modulates a charged particle beam. The system has uncertainties in the governing parameters as well as initial distribution of charged particles. The problem is challenging due to uncertainity, high-dimensional parameter space, limited measurements of the beam etc.
* We investigate different aspects of the problem: estimating forward beam dynamics, inverting the beam dynamics, parameter estimation and control with UQ.
* In [Paper-1](https://www.nature.com/articles/s41598-024-68944-0), we propose two-step unsupervised deep learning framework named as Conditional Latent Autoregressive Recurrent Model (CLARM) for learning the forward spatiotemporal dynamics. The model can generate phase space at various accelerator modules by sampling and decoding the structured latent space representation. The model also forecasts future states (downstream states) of charged particles from past states (upstream states). More about it on the [project page](https://github.com/lanl/clarm).

<p align="center">
  <img src="../images/clarm_lansce.png" width="450" height="260" />
</p>

* In [Paper-2](https://arxiv.org/abs/2408.07847), we use a reverse latent evolution model (CLARM is a special use case of a more broader LEM) to solve the inverse problem of predicting 6D phase space projections across all upstream accelerating sections based on single or multiple downstream phase space measurements as inputs. The proposed model also captures the aleatoric uncertainty of the high-dimensional input data within the latent space. The uncertainity is propagated in the latent space through the temporal learner to estimate the bounds for all upstream predictions, demonstrating the robustness against in-distribution variations in the input data.

  
## Structural health monitoring
1. Out-of-distribution detection/Anomaly detection in aerospace composites: Collecting datasets accommodating all possible damage scenarios is cumbersome, costly, and inaccessible for aerospace applications. In this paper, we have proposed two different self-supervised representation learning approaches to learn the distribution of baseline signals. The trained self-supervised learner is used for delamination prediction with an anomaly detection philosophy. We metholdogies like autoencoders, variational autoencoders, PCA-SVM, ICA-SVM are employed.

2. 
  
* Deep variational filtering for temperature effects in guided wave structural health monitoring
* Physical-knowledge assisted ML for structural health monitoring.
* Supervised DL for guided wave SHM

## 3. Wave propagation analysis and general PDEs
* Physics-informed NN for wave propagation
* Bayesian-optimized PINNs for parameter estimation

## 4. Material informatics
* Composite material property estimation using supervised DL.
* Composite material generation/discovery using generative AI.

## 5. Safety of space habitats
* Leakage estimation in concept space habitats/pressurized habitat systems using adaptive optimization.

## 6. Robotics
* Pipe health monitoring robot
