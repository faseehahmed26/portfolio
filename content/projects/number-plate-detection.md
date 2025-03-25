--- 
title: "Number Plate Detection & Recognition"
description: "Real-time license plate detection and OCR system using TensorFlow Object Detection API"
dateString: Jul 2022 - Sep 2022
draft: false
tags: ["Computer Vision", "TensorFlow", "Object Detection", "OCR", "Transfer Learning", "EasyOCR", "Image Processing", "SSD MobileNet", "Deep Learning", "CUDA"]
showToc: false
weight: 306
cover:
   image: "projects/number-plate-detection/cover.png"
---


### 🔗 [GitHub](https://github.com/faseehahmed26/Number-Plate-Detection)

## Description

* Developed an end-to-end license plate detection and recognition system using TensorFlow Object Detection API and EasyOCR, achieving high accuracy in real-time environments.

* Implemented transfer learning with SSD MobileNet v2 FPN-Lite architecture pre-trained on COCO dataset, fine-tuned for the specific task of license plate detection.

* Created a comprehensive data pipeline including image collection, annotation, preprocessing, and TFRecord generation for efficient model training.

* Optimized model hyperparameters by modifying the pipeline configuration, including learning rate schedules, batch sizes, and anchor box settings for small object detection.

* Engineered a post-processing pipeline that automatically extracts detected license plate regions, applies OCR, and filters text results based on confidence thresholds.

* Built a real-time detection system using OpenCV that processes webcam feed, detects license plates, performs OCR, and logs results to CSV files with corresponding images.

* Implemented model export functionality to multiple formats (TensorFlow SavedModel, TFJS, TFLite) enabling deployment across different platforms and devices.

* Created region-of-interest (ROI) filtering to improve OCR accuracy by analyzing the relative size and position of text within detected license plate regions.

* Designed the system to automatically save detection results with unique identifiers for later auditing and verification purposes.

* Leveraged GPU acceleration through TensorFlow, enabling efficient training and near real-time inference performance on compatible hardware.