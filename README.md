# Semantic Inpainting for Distributed Cross-Modal Integrated Sensing and Communication (ISAC)

**Semantic Inpainting with Multi-Modal Data (e.g., Image + CSI)**  
This repository contains code and models for performing visual inpainting of occluded regions using deep learning, with a focus on leveraging auxiliary sensor modalities such as Wi-Fi CSI (Channel State Information).

---

## Features

- Semantic inpainting with partial or occluded inputs
- Support for image-only and cross-modal setups (e.g., CSI-to-image)
- Encoder-decoder architectures with optional pretrained ViT backbone
- Temporal smoothing and CSI fusion modules
- Visualization tools for input/output comparisons



## Project Structure


## Semantic Inpainting Framework
We consider a wireless network in which each cell consists of a BS, regular wireless terminals (users), and multimodal sensors (e.g., cameras, LiDAR, RF). The cell spans a small-area coverage (tens of meters), with sensors deployed　to monitor the local environment. For simplicity, we assume that sensors are managed by the network operator, which allocates wireless resource blocks b to both terminals and sensors. Terminals transmit data proportionally to their　allocated resources, while only sensors receiving sufficient resources are permitted to transmit. In addition, RF modalities are extracted from communication signals transmitted by both terminals and sensors, providing physical-state observations of　the environment.

![semantic_inpainting_framework](Images/semantic_inpainting.png)


## News

- **[2025-02-08]** Our paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://icmlcn2025.ieee-icmlcn.org/), Congratulations!


---




