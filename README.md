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
├── experiments/   
├── pretrained models/        #  Pretrained components (encoders, inpaintors, and decoders)
├── Images/            　　　　#  Figures for docs
└── README.md
```


## Dataset
Here we thank [Mr. Shoki Ohta](https://scholar.google.com/citations?user=Q75FgBcAAAAJ&hl=ja) for his invaluable efforts in collecting the dataset.

The [dataset](https://huggingface.co/datasets/cheng-chen-ScienceTky/Semantic_Inpainting/tree/main) includes both Wi-Fi CSI and synchronized image sequences. Please refer to the paper for detailed setup.
- **[CSI Data]**: Amplitude values collected from nine sensors are stored in the CSI/ folder.
- **[Image Data]**: Time-sequenced images from each camera are stored in separate folders. All images are resized to 224×224×3 to reduce storage and allow easy feeding into deep models. You may resize them back to any desired resolution.
- **[Format]**: All data are provided as NumPy (.npy) files for easy loading.
- **[Preprocessing]**: The data frames are fully synchronized and pre-processed, allowing direct import for experiments.

You can pull the files straight from Hugging Face and load them into your pipeline without manual downloads. Here we offer an example usage:
```code
!pip install -U huggingface_hub numpy
from huggingface_hub import snapshot_download

local_dir = snapshot_download(
    repo_id="cheng-chen-ScienceTky/Semantic_Inpainting",  # dataset repo
    repo_type="dataset"
)

# Now you'll have:
# local_dir/CSI/amp_*.npy            (CSI amplitudes from 9 sensors)
# local_dir/camera_<id>/*.npy        (224x224x3 image sequences per camera)
```

---

## News
- **[Now]** The code, pretrained models, etc. will be available soon.
- **[2025-09-23]** As requested by many readers, we have released the [dataset](https://huggingface.co/datasets/cheng-chen-ScienceTky/Semantic_Inpainting/tree/main) on Huggingface.
- **[2025-07-28]** Our work was presented at the proceeding of [28th Meeting on Image Recognition and Understanding (MIRU2025)​](https://cvim.ipsj.or.jp/MIRU2025/timetable-en.html).
- **[2025-05-28]** Prof. Nishio and Chen attended the ICMLCN 2025 held in Barcelona, Spain, and Chen gave a [poster presentation](https://drive.google.com/file/d/1cm067bY0UgkVZ4J08-CdYT2SDGj-J6Rr/view?usp=sharing).
- **[2025-02-08]** Our PoC paper is accepted by the proceeding of [IEEE International Conference on Machine Learning for Communication and Networking (ICMLCN) 2025](https://ieeexplore.ieee.org/abstract/document/11140469), Congratulations!


---

## Acknowledgement
This project was conducted under the joint supervision of and [Prof. Takayuki Nishio](https://scholar.google.co.jp/citations?user=hHnMMMkAAAAJ&hl=ja), Institute of Science Tokyo, Japan, and [Prof. Mehdi Bennis](https://scholar.google.com/citations?user=RW4sJu8AAAAJ&hl=en), University of Oulu, Finland.
We also thank [Mr. Shoki Ohta](https://scholar.google.com/citations?user=Q75FgBcAAAAJ&hl=ja), Institute of Science Tokyo, Japan, for his invaluable efforts in collecting the dataset.
Their guidance and support are gratefully acknowledged!



