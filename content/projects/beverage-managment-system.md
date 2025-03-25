---
title: "Beverage Management System"
description: "A real-time inventory tracking system using YOLOv5 and Streamlit"
dateString: 2022
draft: false
tags: ["Computer Vision", "Deep Learning", "YOLOv5", "Streamlit", "Python", "PyTorch", "SQLite", "WebRTC", "Inventory Management"]
showToc: false
weight: 202
cover:
   image: "projects/beverage-system/beverage.jpg"
--- 
### 🔗 [GitHub](https://github.com/faseehahmed26/Cold-Drinks-Inventory-System)
### 🔗 [Live Demo](https://faseehahmed26-cold-drinks-inventory-system-app-g8v3la.streamlit.app/)
### 🔗 [Dataset](https://www.kaggle.com/datasets/faseeh001/cold-drinks-inventory-dataset)

## Description

I built a real-time beverage inventory management system that combines computer vision with a database backend to automate stock tracking. The application uses YOLOv5 object detection to identify different beverage types (Coca-Cola, Sprite, Pepsi, etc.) through a camera feed, automatically updating inventory counts in a SQLite database.

The system features dual access modes - a staff interface for real-time scanning and an admin dashboard for inventory management. I implemented WebRTC for smooth live video streaming with detection speeds as low as 5ms per frame, ensuring the system could operate efficiently even on mobile devices. 

Key technical achievements include:
- Custom-trained YOLOv5 model optimized for beverage recognition with 90% accuracy
- Responsive Streamlit frontend with real-time video processing
- Automated database updates tracking inventory changes by date and product
- Support for both live camera detection and image upload workflows

This project demonstrates practical application of deep learning in retail inventory management, significantly reducing manual counting time and improving accuracy. I also published an article about this project on Medium, explaining the implementation details and development process.