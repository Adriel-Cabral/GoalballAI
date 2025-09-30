# GoalballAI: A Dataset for Player and Ball Detection in Goalball

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## 📖 Overview

This repository contains the dataset introduced in the paper **"GoalballAI: A computer vision dataset for player and ball detection in Goalball"**.

**GoalballAI** is, to the best of our knowledge, **the first publicly available dataset** for object detection in the Paralympic sport of Goalball. It aims to foster research in computer vision for sports analytics, specifically for visually impaired sports, by providing a high-quality annotated benchmark.

> **Abstract:** Computer vision and machine learning have transformed sports analysis, allowing a precise assessment of athletes’ actions, optimizing strategies, and enhancing game understanding. However, the application of these technologies in Goalball, a Paralympic sport for athletes with visual impairments, is limited by the lack of specialized datasets. To address this gap, this paper presents the GoalballAI, to the best of our knowledge, the first public dataset for object detection in Goalball matches, opening new research avenues for automated tactical analysis and performance evaluation in the sport. The dataset was constructed from videos of official games and training sessions, covering both male and female competitions at regional, national, and international levels. GoalballAI comprises 8,000 images with 60,436 annotated instances of two classes ('player' and 'ball') .To establish baselines, we trained YOLOv10s and YOLOv11s. Both models achieved mAP@0.5 > 0.950 for player detection, whereas ball detection was more challenging (mAP@0.5 < 0.610).

## 🗂️ Dataset Download

The GoalballAI dataset is publicly available for download under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

**📥 Download the Dataset Here:** https://drive.google.com/drive/folders/1s9UsrdQGWSpFKEJ6vo7rMM4oKAahXNYN?usp=sharing

### Available Formats:
- **YOLOv8** 
- **COCO** 
- **Pascal VOC**
  
## ✨ Key Features

*   **Scale:** 8,000 images with 60,436 annotated instances.
*   **Classes:** Two object classes: `player` and `ball`.
*   **Diversity:** Sourced from various official competitions (e.g., Paralympic Games, World Championships) and training sessions, featuring both male and female players.
*   **Variability:** Includes different court colors, lighting conditions, player uniforms, and camera resolutions (SD to Full HD).
*   **Annotations:** Bounding box annotations in popular formats (e.g., YOLO, COCO, Pascal Voc).
*   **Baselines:** Provides baseline results using state-of-the-art YOLOv10 and YOLOv11 models.

## 📊 Dataset Composition

| Split       | Images | Player Instances | Ball Instances | Total Instances |
|-------------|--------|------------------|----------------|-----------------|
| Training    | 6,300  | 36,659           | 10,648         | 47,307          |
| Validation  | 1,200  | 7,030            | 2,596          | 9,626           |
| Test        | 500    | 2,978            | 525            | 3,503           |
| **Total**   | **8,000** | **46,667**       | **13,769**     | **60,436**      |

## 🚀 Baseline Models & Results

We established baselines using **YOLOv10s** and **YOLOv11s** models. The fine-tuned models significantly outperformed their generic counterparts pre-trained on COCO.

### Fine-Tuned Model Performance (mAP@0.5)

| Model     | Player Class | Ball Class | Overall (mAP@0.5) |
|-----------|--------------|------------|-------------------|
| YOLOv10s  | 0.963        | 0.602      | 0.783             |
| YOLOv11s  | 0.971        | 0.568      | 0.770             |

Player detection achieved high accuracy, while ball detection remains challenging due to its small size, high speed, and occlusions.

## 🎯 Potential Applications

*   Automated player and ball tracking.
*   Tactical analysis (e.g., defensive formations, shooting zones).
*   Performance evaluation for athletes and coaches.
*   Development of real-time assistive technologies for training.
*   Benchmarking for object detection models in sports.
