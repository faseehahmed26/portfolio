--- 
title: "Flight Fare Predictor"
description: "Machine learning system for predicting flight prices based on travel details"
dateString: "Apr 2022 - Jun 2022"
draft: false
tags: ["Machine Learning", "Random Forest", "Python", "Feature Engineering", "Data Cleaning", "Flask", "Hyperparameter Tuning", "Regression", "Pandas", "Scikit-learn", "Seaborn", "Pickle"]
showToc: false
weight: 303
cover:
   image: "projects/flight-price-predictor/cover.png"
---


### 🔗 [GitHub](https://github.com/faseehahmed26/Flight-Fare-Predictor)
### 🔗 [Live Demo](https://flight-fare-predictor-app.herokuapp.com/)

## Description

* Developed a machine learning system that predicts domestic flight prices with ~80% accuracy using a Random Forest Regression model, enabling travelers to make cost-effective booking decisions.

* Implemented comprehensive data processing techniques for complex temporal features, extracting journey day, month, departure time, arrival time, and flight duration from raw string data.

* Engineered a sophisticated data preprocessing pipeline that handles categorical features through one-hot encoding for airlines, source, and destination, improving model performance.

* Created custom feature extraction for duration data, splitting into hours and minutes components to provide more meaningful input signals for the model.

* Applied feature importance analysis using ExtraTreesRegressor to identify key price determinants, with total stops, journey day, and airline carrier emerging as the most influential factors.

* Optimized the Random Forest model through RandomizedSearchCV, systematically exploring 50 parameter combinations across 10 iterations to reduce prediction error.

* Achieved high model performance metrics with R² score of 0.797, Mean Absolute Error of 1,145 rupees, and Root Mean Square Error of 2,011 rupees on unseen test data.

* Built a user-friendly web interface using Flask that accepts inputs like departure location, destination, travel date, and airline, delivering instant fare predictions.

* Deployed the trained model as a web service using Heroku's cloud platform, making the predictive analytics tool accessible to travelers worldwide.

* Created insightful visualizations of price correlations across airlines, routes, and timing factors to uncover underlying patterns in the pricing data.

