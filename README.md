# IBM_DataScience_Capstone_Project

This project is part of the IBM Data Science Professional Certificate Capstone and focuses on predicting the success of SpaceX's Falcon 9 rocket landings. The goal is to analyze various features of Falcon 9 launches and build machine learning models to predict whether the first stage of a Falcon 9 rocket will successfully land, thus lowering the cost of space missions.

Outline

1. Executive Summary
2. Introduction
3. Methodology
4. Results
5. Conclusion

Project Overview

SpaceX aims to make space travel more affordable by reusing the first stage of its Falcon 9 rockets. This project analyzes the factors that influence the success of Falcon 9 landings and builds predictive models to estimate the likelihood of a successful landing.

Problem Statement

The primary objective is to predict the outcome of Falcon 9 first stage landings using various features like launch site, payload mass, orbit type, and more. Accurate predictions can help reduce the costs associated with space launches by reusing rockets.

Methodology

The methodology includes:

Data Collection: Gathering data from SpaceX's API and web scraping Falcon 9 launch data from Wikipedia.
Data Wrangling: Cleaning, filtering, and formatting the data to prepare it for analysis and modeling.
Exploratory Data Analysis: Using SQL, Pandas, and data visualization tools to understand the relationships within the data.
Data Visualization: Creating visual insights using Matplotlib, Seaborn, and Folium.
Machine Learning: Building and evaluating predictive models using Scikit-learn.
Data Collection

SpaceX API: Collected data on rocket launches, focusing on Falcon 9 missions.
Web Scraping: Additional data was scraped from Wikipedia to fill in gaps and provide comprehensive information on launch outcomes.
Data Wrangling

Filtered the dataset to include only Falcon 9 launches.
Replaced missing values using column means and one-hot encoding for categorical variables.
Created a binary column to classify landing outcomes as successful (1) or unsuccessful (0).
Exploratory Data Analysis

Analyzed the distribution and frequency of launches across different sites and orbits.
Examined the correlation between payload mass and launch success.
Used SQL queries to extract meaningful insights about the launch data.
Data Visualization

Plotted relationships between flight number, payload mass, launch site, and orbit type.
Visualized launch sites and outcomes on interactive maps using Folium.
Created dashboards with Plotly Dash to explore the impact of different features on launch success.
Machine Learning Models

Built predictive models using Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN).
Used GridSearchCV for hyperparameter tuning and model optimization.
Evaluated models based on accuracy, F1 score, and confusion matrices.
Results

The Decision Tree model performed the best, achieving the highest accuracy and F1 score among the tested models.
Launch sites near the equator, like KSC LC-39A, showed the highest success rates, particularly for orbits ES-L1, GEO, HEO, and SSO.
Conclusion

The analysis showed that:

The Decision Tree model is the most effective for predicting Falcon 9 landing outcomes.
Launch sites near the equator benefit from Earth's rotational speed, aiding in successful launches.
Future research should focus on expanding the dataset and exploring more advanced models like XGBoost.
Future Work

Larger Dataset: Incorporating more data to improve the generalizability of the models.
Feature Engineering: Conducting further feature analysis or using Principal Component Analysis (PCA) for better model accuracy.
Advanced Models: Exploring the use of XGBoost or other advanced models to potentially outperform current predictions.
