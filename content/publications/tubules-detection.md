--- 
title: "Tubules Detection on Breast Carcinoma Whole Slide Images"
description: "AI-powered detection system for breast cancer grading using deep learning"
dateString: "Sep 2022"
draft: false
tags: ["Deep Learning", "Computer Vision", "HistomicsUI", "Python", "QuPath", "R2U-Net", "Horovod", "Groovy", "Distributed Training", "Medical Imaging"]
showToc: false
weight: 301
cover:
   image: "publications/tubules-detection/tub3.png"
---


### 🔗 [Publication Abstract](https://cdn.ymaws.com/siim.org/resource/resmgr/mimi22/abstracts/Tubules_Detection_on_Breast_.pdf)

## Research Overview

I presented our groundbreaking research on tubule detection in breast carcinoma whole slide images at SIIM-CMIMI22 (International Conference On Machine Intelligence in Medical Imaging) at Johns Hopkins Hospital, Baltimore, MD. This work addresses a critical component of the Nottingham Breast Cancer Grading system, automating what has traditionally been a tedious manual process for pathologists.

## Technical Approach

Our system employed the R2U-Net CNN architecture, a specialized recurrent residual convolutional neural network optimized for medical image segmentation. The model was trained on two distinct datasets:

* **Public Dataset**: 85 whole slide images (775 x 522) at 40x resolution containing 795 annotated tubules
* **Local Hospital Dataset**: 50 whole slide images (40,000 x 40,000) at 40x resolution with approximately 25,000 tubules from Basavatarakam Indo-American Cancer Hospital in Hyderabad, India


## Distributed Training Innovation

A key innovation in our approach was implementing distributed training using Horovod, an open-source framework that leverages data parallelism to optimize resource allocation:

* Trained the model across 4 GPUs simultaneously
* Achieved 3.9x faster training compared to single-GPU implementation
* Reduced training time from ~27 hours to just 7 hours for 500 epochs

## System Architecture

The end-to-end pipeline consisted of:

1. **Data Preparation**: Pathologists annotated tubules using CADD4MBC (Computer-Aided Detection and Diagnosis for Molecular Breast Cancer), with annotations saved as JSON files
2. **Preprocessing**: Custom scripts using QuPath and Groovy to extract and prepare training data
3. **Model Training**: R2U-Net architecture with distributed training via Horovod
4. **Integration**: Web-based viewer for pathologists to upload, analyze, and review results

## Results

Our model achieved exceptional performance metrics:

| Dataset | Training F1 Score | Training Mean IOU | Testing F1 Score | Testing Mean IOU |
|---------|-------------------|-------------------|------------------|-----------------|
| Public  | 0.9974            | 0.9070            | 0.9293           | 0.7537          |
| KMIT    | 0.9962            | 0.9116            | 0.9105           | 0.8053          |

These results demonstrate that deep learning approaches can effectively automate tubule detection with high accuracy, potentially reducing pathologists' workload and improving diagnostic consistency in breast cancer grading.

<!-- ![Visualization of Results](/publications/tubules-detection/visualization.png) -->

## Impact

This research represents a significant advancement in computational pathology, offering:

* Faster and more consistent tubule detection for breast cancer grading
* Reduced burden on pathologists for manual identification
* A scalable framework that can be extended to other histopathological features
* Integration with existing clinical workflows through web-based platforms

The project demonstrates how deep learning can enhance cancer diagnostics while maintaining the critical role of pathologists in the evaluation process.
![](/publications/tubules-detection/tub3.png#center)

![](/publications/tubules-detection/horovord.png)
