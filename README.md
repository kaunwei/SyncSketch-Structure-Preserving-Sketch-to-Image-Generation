# SyncSketch-Structure-Preserving-Sketch-to-Image-Generation
SyncSketch is a research-driven Generative AI framework designed to convert hand-drawn furniture sketches into photorealistic renders while strictly preserving the original geometric structure.<br>

# Colab File Link

https://colab.research.google.com/drive/1e4Ez9ltLUzM9R3fbghbBel1Ukp0TcTHS?usp=sharing <br>

![WhatsApp Image](https://raw.githubusercontent.com/USERNAME/REPO/main/images/whatsapp-image.jpeg)

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


# Dataset

Sketch2Image Furniture Dataset (Kaggle)<br>
Categories: Chairs, Tables, Cabinets<br>
<br>
# Dataset link:
https://www.kaggle.com/datasets/robinrausch/sketch2image-dataset-furniture<br>
<br>
# Results (Highlights)

- Average edge alignment fidelity: 84.5%
- Significant improvement over GAN-based methods
- Strong preservation of thin and precise structures
- Reduced inference time compared to standard diffusion pipelines

 # Technologies Used

- Python
- PyTorch
- Stable Diffusion
- ControlNet
- OpenCV (Canny Edge Detection)
- Diffusion Models

# Author
Ayesha Khan
AI/ML Researcher

For any inquiries, please feel free to contact me via email.
ayesha156781@gmail.com
