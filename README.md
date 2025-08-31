<div align=center>
  <h1>
  DDPM and DDIM
  </h1>
  <p>
    <a href=https://mhsung.github.io/kaist-cs492d-fall-2025/ target="_blank"><b>KAIST CS492(C): Diffusion and Flow Models (Fall 2025)</b></a><br>
    Programming Assignment 1
  </p>
</div> 

<div align=center>
  <p>
    Instructor: <a href=https://mhsung.github.io target="_blank"><b>Minhyuk Sung</b></a> (mhsung [at] kaist.ac.kr)<br>
    TA: <a href=https://dvelopery0115.github.io target="_blank"><b>Yunhong Min</b></a>  (dbsghd363 [at] kaist.ac.kr)<br>
    Credit: <a href=https://63days.github.io target="_blank"><b>Juil Koo</b></a>  (63days [at] kaist.ac.kr) & <a href=https://hieuristics.xyz/ target="_blank"><b>Nguyen Minh Hieu</b></a>  (hieu1052k3 [at] gmail.com)<br>
  </p>
</div>

<div align=center>
   <img src="./assets/ddpm_vis.gif">
</div>


## Abstract
Denoising Diffusion Probabilistic Models (DDPM) are a generative modeling framework that learns to reverse a predefined diffusion process. By gradually corrupting data with Gaussian noise in the forward process and training a neural network to denoise step by step, DDPM is able to synthesize high-quality samples from pure noise. The objective in DDPM is to predict the injected noise at each timestep, and the reverse process is modeled as a stochastic Markov chain.

Denoising Diffusion Implicit Models (DDIM) build on the same noise-prediction model but introduce more generalized non-Markovian forward process. This modification provides an alternative trajectory for sample generation, often reducing the number of inference steps required while maintaining competitive sample quality. In this way, DDIM highlights the flexibility of diffusion models in trading off efficiency and fidelity.

In this first assignment, we will implement DDPM and DDIM step by step on a 2D toy dataset, compare their sampling behaviors, and gain practical experience with the core components of diffusion-based generative modeling.

## Setup

Clone this repository and upload the notebook file `DDPM_DDIM.ipynb` to [Google Colab](https://colab.research.google.com).  
**All instructions—including task descriptions and submission guidelines—are provided in the notebook file. Please follow them carefully to complete the tasks.**
