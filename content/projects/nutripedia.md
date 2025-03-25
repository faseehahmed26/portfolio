---
title: "NutriPedia - Food Recognition & Calorie Estimation"
description: "An AI-powered food recognition system with calorie estimation"
dateString: 2023
draft: false
tags: ["Computer Vision", "Deep Learning", "Inception-V3", "Mask R-CNN", "Food Recognition", "Nutrition", "Google Cloud", "TensorFlow", "PyTorch", "SQL"]
showToc: false
weight: 203
cover:
   image: "projects/nutripedia/system-design.jpg"
--- 
### 🔗 [GitHub](https://github.com/faseehahmed26/nutripedia)

## Description

NutriPedia is an advanced food recognition and nutrition tracking platform that helps users maintain healthier eating habits. The system uses deep learning to identify food items from images, calculate portion sizes, and provide detailed nutritional information including calories, macronutrients, and vitamins.

I implemented a hybrid architecture combining Inception-V3 and Mask R-CNN models to achieve superior food classification accuracy. The Inception-V3 model, chosen for its computational efficiency (replacing 5×5 convolutions with two 3×3 convolutions reduced computation cost by 33%), achieved 93.7% accuracy on the FOOD-101 dataset. The Mask R-CNN component enables precise food item segmentation, allowing for accurate portion size estimation.

Key technical features include:
- A comprehensive data pipeline that stores images in Google Cloud Storage and manages metadata in SQL databases
- Implementation of a "FlyWheel" concept where user contributions continuously improve model accuracy
- Automated calorie estimation based on food type identification and estimated portion sizes
- Cloud-based architecture designed for scalability with thousands of food items

This project addresses the growing demand for automated food recognition systems as people become more health-conscious and seek tools to support balanced diets and prevent disordered eating. The system currently recognizes and analyzes 6 food categories with plans to expand to a more comprehensive database.