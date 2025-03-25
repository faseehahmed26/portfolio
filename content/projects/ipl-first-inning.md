--- 
title: "IPL First Innings Score Predictor"
description: "Machine Learning model to predict cricket match scores using historical data"
dateString: "Jun 2022 - Aug 2022"
draft: false
tags: ["Machine Learning", "Regression", "Python", "Flask", "Ridge Regression", "Lasso Regression", "Pandas", "Scikit-learn", "Data Cleaning", "Feature Engineering", "Model Deployment", "Sports Analytics"]
showToc: false
weight: 306
cover:
   image: "projects/ipl-first-inning/before.png"
---


### 🔗 [GitHub](https://github.com/faseehahmed26/IPL_First_Innings_Score)
### 🔗 [Live Demo](https://ipl-score-predictor-app.herokuapp.com/)

## Description

* Developed a machine learning system that predicts Indian Premier League (IPL) cricket first innings scores with a Root Mean Square Error (RMSE) of approximately 20 runs using Ridge and Lasso regression models.

* Engineered a comprehensive data preprocessing pipeline that handles categorical features through one-hot encoding, addressing the complexity of team matchups in cricket analytics.

* Implemented temporal data splitting strategy by using pre-2017 matches for training and post-2017 matches for testing, ensuring robust model evaluation that mimics real-world prediction scenarios.

* Applied feature selection by filtering for consistent teams across seasons and removing irrelevant columns, improving model generalization and reducing noise in the prediction system.

* Optimized model hyperparameters using GridSearchCV with 5-fold cross-validation, systematically evaluating 12 different alpha values to find the optimal regularization strength.

* Conducted comparative analysis between Ridge and Lasso regression models, with Ridge regression achieving slightly better performance (MSE: 403.2 vs 414.6) for this specific prediction task.

* Created error distribution visualizations to understand prediction patterns, revealing normally distributed errors centered around zero with most predictions falling within ±20 runs.

* Built a Flask web application with an intuitive interface allowing users to select match conditions like batting team, bowling team, current score, and overs played to generate score predictions.

* Deployed the trained model as a web service using Heroku's cloud platform, making the predictive analytics tool accessible to cricket fans and analysts worldwide.

* Serialized both Ridge and Lasso models using pickle, enabling fast loading and prediction without retraining, while maintaining the option to switch between models as needed.

![](/projects/ipl-first-inning/after.png#center)