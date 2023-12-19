# Drone Detection Project - SkyGuard Y5
<img src="https://github.com/muqeet-here/SkyGuard-Y5/blob/main/images/Image.png" alt="Drone">
## Overview

This repository contains the implementation of a Printed Circuit Board (PCB) defect detection system using YOLOv8, a state-of-the-art object detection model. The objective is to identify and classify defects on PCBs, providing a reliable tool for quality control in manufacturing processes.

## Model Optimization

To enhance the efficiency and practicality of the model, several optimizations were performed:

### 1. Mean Average Precision (mAP) Improvement

Implemented techniques to improve the Mean Average Precision of the YOLOv8 model. This ensures more accurate and reliable detection of defects on PCBs.

### 2. Model Size Reduction

Reduced the model size to 22 MB, enhancing the deployment feasibility of the model on resource-constrained environments.

## Data Preprocessing

1. Utilized the Roboflow platform for efficient annotation and preprocessing of the PCB defect dataset. Dataset available [here](https://universe.roboflow.com/hubei-university-of-technology-rmbpi/pcb-ecjga).
2. Converted the annotated dataset into the YOLOv8 format for compatibility with the chosen model architecture.

## Training Process in Colab

1. Utilized the YOLOv8 custom training notebook in Colab for efficient and scalable training. Access the notebook [here](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/train-yolov8-object-detection-on-custom-dataset.ipynb).
2. Configured the notebook to utilize the GPU for faster training.
3. Incorporated necessary hyperparameter tuning for optimal model performance.
4. Monitored training progress and visualized results to ensure model convergence.

## Evaluation

Conducted thorough evaluation metrics analysis to validate the effectiveness of the trained YOLOv8 model. This includes precision, recall, and F1-score metrics to assess the model's accuracy in detecting PCB defects.

## Defect Classes

This project encompasses a broader spectrum of defects compared to previous researches. The eight defect classes include:
1. False Copper
2. Missing Hole
3. Mousebite
4. Open Circuit
5. Pinhole
6. Scratch
7. Short Circuit
8. Spur

## Previous Researches

While previous researches typically focused on six defect classes, our project extends the scope to include the additional defect classes of False Copper and Spur, providing a more comprehensive defect detection solution.

## GitHub Repository

Feel free to explore the code, documentation, and resources in this repository. If you have any questions or suggestions, please don't hesitate to reach out.

**Repo Name: PCB-YOLOv8-Defect-Detection**

Feel free to modify the repository name based on your preferences. This repository will serve as a centralized hub for your project.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
