# Semantic Inpainting for Distributed Cross-Modal Integrated Sensing and Communication (ISAC)

This repo provides code and pretrained models for a semantic-space inpainting framework that unifies sensing and communication across modalities such as RGB images and Wi-Fi CSI.

---


## Semantic Inpainting Framework
We considered a semantic inpainting framework where missing sensing modalities are inpainted via self-supervised semantic-space aggregation, providing the receiver with comprehensive target information.
<img src="Images/semantic_inpainting.png" alt="semantic_inpainting_framework" width="700"/>

### Features
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

## Project Structure
```text
semantic-inpainting-framework/
├── code/            # Encoders, decoders, projection heads
├── data/              # Pre-/post-processing scripts
├── experiments/       # Training & evaluation pipelines
├── pretrained models/        # Pretrained weights (optional)
├── Images/            # Figures for docs
└── README.md
```

---

## News
- **[2025-07-28]** Our paper is to be presented at the proceeding of [28th Meeting on Image Recognition and Understanding (MIRU2025)​](https://cvim.ipsj.or.jp/MIRU2025/timetable-en.html).
- **[2025-07-28]** Chen and Prof.Nishio attended the ICMLCN 2025 held in Barcelona, Spain, and Chen gave a [poster presentation](https://drive.google.com/file/d/1cm067bY0UgkVZ4J08-CdYT2SDGj-J6Rr/view?usp=sharing).
- **[2025-02-08]** Our paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://icmlcn2025.ieee-icmlcn.org/), Congratulations!







