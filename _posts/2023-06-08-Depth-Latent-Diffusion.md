---
layout: page
title: Depth Latent Diffusion
---

Trained a conditional Latent-Diffusion Model for monocular depth estimation on the NYU dataset. 

- First trained a VQ-VAE to learn the latent space of the depth map conditioned on the RGB image

- Once the VQ-VAE was trained, its weights were frozen and used to generate the latent representation of the depth map for the forward diffusion process and denoising while being conditioned on the RGB image

- Experimented with different forms of RGB conditional block aggregation with the U-Net architecture, including Spatial Rescaler concatenation and using DINOv2 to extract meaningful features from the RGB image  

- The model was trained on the NYU dataset

You can find the project report here [[Link](https://drive.google.com/file/d/1AY2GY7jdtdnQ_bIc3K0ELCpPsG4NxzEH/view?usp=sharing)]


<!-- ![NYU_progrssing_denoising](/assets/progressive_denoising.png) <br /> <br /> -->
![NYU_progrssing_denoising](/assets/DGM_progressive_denoising.png) 
*Progressive denoising of the latent space conditioned on the RGB image to generate the depth map*


<!-- <br /> <br/> -->
![NYU_progrssing_denoising](/assets/DGM_results_1.png) 
*Result comparison between the spatial rescaler and using DINOv2 for RBG conditioning*



