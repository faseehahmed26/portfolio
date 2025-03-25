--- 
title: "Web-based Mitosis Detection on Breast Cancer WSI"
description: "Advanced object detection models for automating mitotic figure identification"
dateString: "Oct 2022"
draft: false
tags: ["Deep Learning", "Computer Vision", "Object Detection", "PyTorch", "FasterRCNN", "YOLOv5", "HistomicsTK", "Detectron2", "Medical Imaging", "Cancer Detection"]
showToc: false
weight: 302
cover:
   image: "publications/mitosis-detection/tile_pred.png"
---

<userStyle>Normal</userStyle>

### 🔗 [Publication Link](https://thesai.org/Publications/ViewPaper?Volume=13&Issue=10&Code=IJACSA&SerialNo=62)

## Research Summary

This research, published in the International Journal of Advanced Computer Science Applications (IJACSA), presents an end-to-end web-based deep learning system for detecting mitotic figures in breast cancer whole slide images (WSI). Mitotic count is a critical component of the Nottingham Breast Cancer Grading system, but manual counting is time-consuming and subject to inter-observer variability.

## Model Comparison

We implemented and compared two state-of-the-art object detection architectures:

1. **FasterRCNN**: A two-stage detector implemented with PyTorch and Detectron2
2. **YOLOv5**: A single-stage detector known for its speed and accuracy

![](publications/mitosis-detection/tiff_pred.png)

Our comparative analysis focused on both accuracy and computational efficiency to identify the most practical solution for clinical deployment.

## Dataset and Training

The training process utilized:

* 56,258 annotated tiles extracted from whole slide images
* 45,006 tiles for training and 11,251 for testing
* High-resolution input (40x magnification)
* Rigorous data augmentation to improve model generalization

![](/publications/mitosis-detection/training.png)

## Performance Analysis

The YOLOv5 model demonstrated superior performance across all key metrics:

| Model      | F1 Score | Training Time | Precision | Recall |
|------------|----------|---------------|-----------|--------|
| FasterRCNN | 77%      | 10h 46m       | 73%       | 81%    |
| YOLOv5     | 84%      | 5h 28m        | 82%       | 86%    |

This represents both higher accuracy and approximately half the training time, making YOLOv5 the preferred model for this application.

![](/publications/mitosis-detection/comparison.png)

## Web Platform Integration

A key innovation of our work was the integration with CADD4MBC, a web-based digital pathology platform that enables:

1. WSI upload and management
2. Annotation tools for ground truth creation
3. Automatic mitosis detection using our trained models
4. Result visualization and validation

![](/publications/mitosis-detection/platform.png)

## Detection Results

Our system successfully detected mitotic figures in complex histopathological images with high accuracy, distinguishing them from similar-appearing structures that often confuse human observers.


## Clinical Impact

This research makes several important contributions to computational pathology:

* Reducing the time required for mitosis counting from hours to minutes
* Improving consistency and reducing inter-observer variability
* Providing an accessible web-based platform that integrates with existing clinical workflows
* Demonstrating the superiority of YOLOv5 for this specific medical imaging application

The web-based nature of our solution makes it particularly valuable for remote consultations and collaborative diagnostics, potentially expanding access to expert pathology services.


![](/mitosis-detection/mit_res.png#center)
