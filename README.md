# Semantic Inpainting for Distributed Cross-Modal Integrated Sensing and Communication (ISAC)

This repo provides code and pretrained models for a semantic-space inpainting framework that unifies sensing and communication across modalities such as RGB images and Wi-Fi CSI.

---


## Semantic Inpainting Framework
We considered a semantic inpainting framework where missing sensing modalities are inpainted via **self-supervised semantic-space aggregation**, providing the receiver with comprehensive target information.
<img src="Images/semantic_inpainting.png" alt="semantic_inpainting_framework" width="700"/>

### Features
- **Cross-ModalSemantic Inpainting with Robust Occlusion-Free Support (robustness)**  
  Restore masked or occluded regions using self-supervised cross-modal context.

- **Flexible Design with Optional Pretrained Architectures for Multiple Downstream Tasks (generalibility)**  
  Semantic Encoder(s) → Semantic Inpaintor (Projection) → Downstream Decoder(s)
  <br>Reuse components across **versatile tasks**, here we give three examples:
  - Image Inpainting  
  - Future CSI Prediction  
  - Human Count Estimation
  
- Compress

---

## Project Structure (in progress...)
```text
semantic-inpainting-framework/
├── code/                     #  Encoders, inpaintors, and decoders
|     ├── Step 3: Pretraining for Downstream Decoders
|     ├── Step 2: Pretraining for Semantic Inpaintors (projection heads)
|     └── Step 1: Pretraining for Semantic Encoders
├── data/                     # Pre-/post-processing scripts
├── experiments/              # Training & evaluation pipelines
├── pretrained models/        # Pretrained components
├── Images/            　　　　# Figures for docs
└── README.md
```

---

## News
- **[Now]** We are working on a journal paper extension. The manuscript, code+data, and pretrained models will be released soon.
- **[2025-07-28]** Our paper is to be presented at the proceeding of [28th Meeting on Image Recognition and Understanding (MIRU2025)​](https://cvim.ipsj.or.jp/MIRU2025/timetable-en.html).
- **[2025-05-28]** Chen and Prof. Nishio attended the ICMLCN 2025 held in Barcelona, Spain, and Chen gave a [poster presentation](https://drive.google.com/file/d/1cm067bY0UgkVZ4J08-CdYT2SDGj-J6Rr/view?usp=sharing).
- **[2025-02-08]** Our paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://icmlcn2025.ieee-icmlcn.org/), Congratulations!


---

## Acknowledgement
This project was conducted under the joint supervision of [Prof. Mehdi Bennis](https://scholar.google.com/citations?user=RW4sJu8AAAAJ&hl=en), University of Oulu, Finland, and [Prof. Takayuki Nishio](https://scholar.google.co.jp/citations?user=hHnMMMkAAAAJ&hl=ja), Institute of Science Tokyo, Japan.
Their guidance and support are gratefully acknowledged!



