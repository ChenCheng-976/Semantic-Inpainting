# Semantic Inpainting for Distributed Cross-Modal Integrated Sensing and Communication (ISAC)

**Semantic Inpainting with Multi-Modal Sensory Data (e.g., Image + CSI)**  
This repository contains code and models for performing visual inpainting of occluded regions using deep learning, with a focus on leveraging auxiliary sensor modalities such as Wi-Fi CSI (Channel State Information).

---


## Semantic Inpainting Framework
We consider a wireless network in which each cell consists of a BS, regular wireless terminals (users), and multi-modal sensors (e.g., cameras, LiDAR, RF). The cell spans a small-area coverage (tens of meters), with sensors deployed to monitor the local environment. For simplicity, we assume that sensors are managed by the network operator, which allocates wireless resource blocks \( b \) to both terminals and sensors. Terminals transmit data proportionally to their allocated resources, while only sensors receiving sufficient resources are permitted to transmit. In addition, RF modalities are extracted from communication signals transmitted by both terminals and sensors, providing physical-state observations of the environment.
<img src="Images/semantic_inpainting.png" alt="semantic_inpainting_framework" width="700"/>



## Features
- **Semantic Inpainting with Occlusion Support**  
  Restore masked or occluded regions using self-supervised cross-modal context.
  
- **Single- & Cross-Modal Compatibility**  
  Works in both single-modality (e.g., image-only) and cross-modality (e.g., CSI-to-image) settings.
  
- **Flexible design with Pretrained Modular Architectures**  
  *Semantic Encoders* → *Semantic Inpaintor (Projection)* → *Downstream Decoder*  
  <br>Reuse components across Versatile tasks:
  - Image Inpainting  
  - Future CSI Prediction  
  - Human Count Estimation

---




## News
- **[2025-07-08]** Our paper is to be presented at the proceeding of [28th Meeting on Image Recognition and Understanding (MIRU2025)​]([https://icmlcn2025.ieee-icmlcn.org/](https://cvim.ipsj.or.jp/MIRU2025/timetable-en.html).
- **[2025-02-08]** Our paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://icmlcn2025.ieee-icmlcn.org/), Congratulations!







