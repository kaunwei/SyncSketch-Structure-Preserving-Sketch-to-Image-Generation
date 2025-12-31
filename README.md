# SyncSketch-Structure-Preserving-Sketch-to-Image-Generation
SyncSketch is a research-driven Generative AI framework designed to convert hand-drawn furniture sketches into photorealistic renders while strictly preserving the original geometric structure.<br>
# Project Summary

SyncSketch is a Generative AI project focused on converting hand-drawn furniture sketches into photorealistic images while strictly preserving the original geometric structure.<br><br>

Most existing GAN and diffusion-based models introduce unwanted distortions when generating realistic images from sketches. This project addresses that limitation by enforcing the sketch as a hard structural constraint during the diffusion process, making it suitable for industrial and design-oriented use cases. <br>

# Key Concept <br>

The core idea is to guide the diffusion model using structural information extracted from the input sketch. A Canny edge map is used to ensure that textures, lighting, and materials are generated only within the exact boundaries of the original sketch.<br>

This approach minimizes creative deviation and prevents common issues such as altered proportions or missing components.<br>

# Method Overview

- Input: Hand-drawn furniture sketch
- Structural Guidance: Canny edge extraction
- Model: Stable Diffusion v1.5 with ControlNet
- Optimization: Tuned conditioning scale for strong geometry preservation
- Inference: Faster sampling using UniPC Multistep Scheduler

