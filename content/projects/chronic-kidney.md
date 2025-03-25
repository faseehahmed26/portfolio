---
title: "Chronic Kidney Disease Predictor"
description: "A MERN stack application for early CKD detection using machine learning"
dateString: May 2022 - Aug 2022
draft: false
tags: ["Machine Learning", "Healthcare", "MERN Stack", "Python", "React", "MongoDB", "Flask", "Random Forest", "XGBoost"]
showToc: false
weight: 105
cover:
   image: "projects/chronic-kidney/ckd_speed.gif"
--- 
### 🔗 [GitHub](https://github.com/faseehahmed26/Kidney-Detection)

## Description

I developed a comprehensive web application for early detection of Chronic Kidney Disease (CKD) using machine learning algorithms. This healthcare tool addresses the critical need for timely CKD diagnosis, as early detection significantly improves treatment outcomes for a condition that often progresses silently until advanced stages.

The system utilizes the UCI Machine Learning Repository's CKD dataset, which I preprocessed to handle the significant number of missing values typical in real-world medical data. I implemented an intelligent data completion algorithm that identifies the most similar complete samples to accurately fill missing values for each incomplete record.

Key technical aspects include:

- **Advanced ML Implementation**: Trained and evaluated multiple classification models, with Random Forest achieving exceptional 99.75% diagnostic accuracy
- **Full-Stack Development**: Built a complete MERN stack application with React frontend, Express/Node.js backend, and MongoDB database
- **Intuitive User Interface**: Designed a clear, accessible interface for healthcare professionals to input patient biomarkers and receive instant risk assessments
- **Secure Data Handling**: Implemented proper protocols for managing sensitive medical information in compliance with best practices

The application allows clinicians to input various patient parameters such as blood pressure, blood glucose, albumin levels, and other key biomarkers to receive an immediate assessment of CKD risk. This tool serves as a valuable clinical decision support system, helping healthcare providers identify at-risk patients who might benefit from earlier intervention and specialized care.