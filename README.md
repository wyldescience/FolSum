<p align="center">
  <img src="https://github.com/user-attachments/assets/20f4e63c-f9c4-494d-b0da-6dd16d9239a4" width="450">
</p>

<h1 align="center">

<p align="center">
Automated detection and counting of <i>Folsomia candida</i> nymphs using YOLOv8
</p>

---

## Overview

**FolSum** is a deep-learning pipeline for automated detection and counting of *Folsomia candida* nymphs from arena images using the Python [Ultralytics YOLOv8 framework](https://github.com/ultralytics/ultralytics).  
The workflow was developed and implemented in Google Colab.

The pipeline includes:

1. automatic arena cropping  
2. tiling of cropped images  
3. YOLOv8-based nymph detection  
4. recombination of detections across overlapping tiles using **non-maximum suppression (NMS)**  
5. validation against manual counts

The model was trained on manually annotated image tiles and validated on an independent set of unseen container images spanning a broad range of offspring densities. The population containers consited of a layers of moistened plaster-paris/ activated charcoal which had a lot of variation in surface texture and lighting (some cases some mold growth) but the model performs very well to distinguish small springtail nymphs and get counts (see validation output and also citation for more details on methods).

Here is an example of a cropped image with an overlay of bounding boxes from model:

<p align="center">
<img src = "https://github.com/user-attachments/assets/ef7373a2-6337-48dc-bc60-2801039bacd5" width = "450">
</p>

---

## Repository contents

- `model/` — trained model weights  
- `scripts/` — Python scripts for preprocessing, inference, and validation  
- `notebooks/` — notebooks used for model training and validation analysis  
- `validation/` — validation data and summary outputs  
- `example_data/` — example images and predictions  

---

## Usage

This repository provides:

- trained YOLOv8 model weights  
- Python scripts used for preprocessing, inference, and validation  
- example data for reproducing the counting workflow  

The pipeline was originally developed and run in **Google Colab**, but the scripts can also be executed locally in a Python environment with the required dependencies installed.

---

## Citation

If you use FolSum in your work, please cite:

*Miller, SM., Wylde, Z., & Bonduriansky, R.(2026). [Maternal senescence broadly reprograms gene expression in offspring]*
https://doi.org/10.64898/2026.04.28.720237
---
