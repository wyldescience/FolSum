
<p align="center">
  <img src="https://github.com/user-attachments/assets/20f4e63c-f9c4-494d-b0da-6dd16d9239a4" width="450">
</p>

<h1 align="center">

<p align="center">
Automated detection and counting of <i>Folsomia candida</i> nymphs using YOLOv8.

  **FolSum** is a deep-learning pipeline for automated detection and counting of *Folsomia candida* nymphs from arena images using YOLOv8.

</p>

## Overview

FolSum was developed to quantify offspring number from images of springtail population containers. The workflow includes:

1. automatic arena cropping  
2. tiling of cropped images  
3. YOLOv8-based nymph detection  
4. recombination of detections across overlapping tiles (NMN- Non Maximum Supression)  
5. validation against manual counts

The model was trained on manually annotated image tiles and validated on an independent set of unseen container images spanning a broad range of offspring densities.

## Repository contents

- `model/` — trained model weights
- `scripts/` — Python scripts for preprocessing, inference, and validation
- `notebooks/` — notebooks used for training and plotting validation results
- `validation/` — validation data and summary outputs
- `example_data/` — example images and predictions

## Installation

### Option 1: pip
```bash
pip install -r requirements.txt
