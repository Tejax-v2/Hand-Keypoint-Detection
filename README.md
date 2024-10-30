# Car Components Segmentation with YOLOv11

This repository contains a fine-tuned YOLOv11 model for segmenting various car components. The model is trained on a Custom Dataset from Roboflow Universe and can be used to detect components such as hood, windows, doors, lights, etc in images.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Model Training](#model-training)
- [Credits](#credits)

---

## Overview

The goal of this project is to create a deep learning model capable of accurately identifying and localizing distinct datapoints on hand. Leveraging YOLOv11's state-of-the-art architecture, the model can detect 21 distinct keypoints with high precision, making it suitable for use in gesture controls in Robotics and AR/VR.

## Dataset

The model was trained on the Ultralytics Hand-Keypoints Dataset, which includes 26,768 labeled images of hands in various lighting conditions, occlusions and surroundings.

### Classes

The dataset contains a single class `hand`. All the keypoints are annotated within the bounding box for hand.

## Installation

To use this project, ensure you have Python and the necessary dependencies installed. Follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Tejax-v2/Hand-Keypoint-Detection.git
    cd Hand-Keypoint-Detection
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
4. **Dataset Preparation**:
   The dataset is downloaded on the go when using the configurations listed in data.yaml file, while starting the model training.

## Model Training

The model is trained using YOLOv11, with adjustments to hyperparameters specific to detecting keypoints. 

Follow the notebook `YOLOv11-Keypoint-Detection.ipynb` for further instructions

## Credits
- Dataset: [ElectroCom61](https://docs.ultralytics.com/datasets/pose/hand-keypoints/)
- Reference: [Roboflow](https://docs.ultralytics.com/datasets/pose/hand-keypoints/)
- Model: [Ultralytics](https://github.com/ultralytics/ultralytics)
