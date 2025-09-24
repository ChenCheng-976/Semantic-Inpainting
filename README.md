# Semantic Inpainting for Distributed Cross-Modal Integrated Sensing and Communication (ISAC)

This repo provides the dataset, code and pretrained models for a semantic-space inpainting framework that unifies sensing and communication across modalities such as RGB images and Wi-Fi CSI.

---


## Semantic Inpainting Framework
We considered a semantic inpainting framework where missing sensing modalities are inpainted via **self-supervised semantic-space aggregation**, providing the receiver with comprehensive target information.
<img src="Images/semantic_inpainting.png" alt="semantic_inpainting_framework" width="700"/>



## Project Structure (in progress...)
```text
semantic-inpainting-framework/
├── code/
├── data/
├── experiments/   
├── pretrained models/        #  Pretrained components (encoders, inpaintors, and decoders)
├── Images/            　　　　#  Figures for docs
└── README.md
```

---

## News
- **[Now]** As requested by several readers, we have released the dataset. The code and pretrained models will be made available shortly.
- **[2025-07-28]** Our work was presented at the proceeding of [28th Meeting on Image Recognition and Understanding (MIRU2025)​](https://cvim.ipsj.or.jp/MIRU2025/timetable-en.html).
- **[2025-05-28]** Prof. Nishio and Chen attended the ICMLCN 2025 held in Barcelona, Spain, and Chen gave a [poster presentation](https://drive.google.com/file/d/1cm067bY0UgkVZ4J08-CdYT2SDGj-J6Rr/view?usp=sharing).
- **[2025-02-08]** Our PoC paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://ieeexplore.ieee.org/abstract/document/11140469), Congratulations!


---

## Acknowledgement
This project was conducted under the joint supervision of and [Prof. Takayuki Nishio](https://scholar.google.co.jp/citations?user=hHnMMMkAAAAJ&hl=ja), Institute of Science Tokyo, Japan, and [Prof. Mehdi Bennis](https://scholar.google.com/citations?user=RW4sJu8AAAAJ&hl=en), University of Oulu, Finland.
Their guidance and support are gratefully acknowledged!



