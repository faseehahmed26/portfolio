---
title: "NutriPedia - Food Recognition & Calorie Estimation"
description: "An AI-powered food recognition system with calorie estimation"
dateString: 2023
draft: false
tags: ["Computer Vision", "Deep Learning", "Inception-V3", "Mask R-CNN", "Food Recognition", "Nutrition", "Google Cloud", "TensorFlow", "PyTorch", "SQL","OpenAI","GPT"]
showToc: false
weight: 203
cover:
   image: "projects/nutripedia/system-design.jpg"
--- 
##### 🔗 [GitHub](https://github.com/faseehahmed26/nutripedia)

## Description


**NutriPedia** is a cutting-edge multimodal AI platform designed to empower users with smarter food recognition and detailed nutrition tracking, helping them make informed dietary choices effortlessly. By simply uploading a picture of a meal, users receive an accurate breakdown of portion size, caloric content, macronutrients, and vitamins—instantly and intelligently.

#### 🔍 Core Technology

The system leverages a hybrid deep learning architecture combining **Inception-V3** and **Mask R-CNN** to deliver high-precision food classification and segmentation.

- **Inception-V3**: Known for its computational efficiency, it replaces traditional 5×5 convolutions with two 3×3 layers, reducing computational complexity by 33%. It achieves **93.7% classification accuracy** on the FOOD-101 dataset.
- **Mask R-CNN**: Used for precise segmentation of individual food items, enabling accurate **portion size estimation**—a key factor for real-world calorie computation.

#### ⚙️ Backend & Architecture

NutriPedia includes a robust cloud-based infrastructure:

- 🗂️ **Google Cloud Storage** for image storage  
- 🧠 **SQL databases** for managing metadata and nutrition information  
- 🔄 **Flywheel Learning Mechanism**: A self-reinforcing loop where user interactions continuously improve model accuracy over time

#### 📊 Key Features

- Automated calorie estimation based on food type and portion size
- Seamless integration of computer vision with NLP via GPT-3.5 for natural, user-friendly summaries
- Scalable architecture designed to support thousands of food categories
- Currently supports **6 core food categories**, with plans for broader dataset expansion

#### 💬 Example Output (via GPT-3.5)

> “Your meal contains roughly 400 calories, with a healthy balance of carbohydrates and fiber. It’s a great post-workout option to restore energy levels and support digestion.”

#### 🎯 Real-World Impact

NutriPedia addresses the growing global need for tools that support healthier lifestyles. As health awareness rises, so does the demand for smart, automated nutrition tracking. NutriPedia is poised to become a valuable companion for individuals aiming to monitor diet, prevent disordered eating, and maintain balanced nutrition—one photo at a time.