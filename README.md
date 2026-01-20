# Applied Data Science Capstone

## Overview

This Applied Data Science Capstone Project focuses on predicting the successful landing of the **Falcon 9 first stage** using data analytics and machine learning techniques.

SpaceX has revolutionized commercial space travel by significantly reducing launch costs. While traditional launch providers charge upwards of $165 million per launch, SpaceX advertises Falcon 9 launches at approximately $62 million. A major contributor to this cost reduction is the **reusability of the Falcon 9 first stage**.

By accurately predicting whether the first stage will successfully land, this project helps estimate launch costs more effectively and provides valuable insights for organizations competing with SpaceX in commercial launch contracts.

---

## Objectives

The project is organized into multiple modules, each building upon the previous one, culminating in a robust predictive model for Falcon 9 landing success.

---

## Project Workflow

### 1. SpaceX API Data Collection and Data Wrangling
- Retrieved historical Falcon 9 launch data using GET requests to the SpaceX REST API
- Collected launch details including payload mass, launch site, rocket configuration, orbit type, and landing outcomes
- Cleaned and formatted the data by handling missing values, correcting inconsistencies, and preparing it for analysis

### 2. Web Scraping Falcon 9 Launch Records
- Scraped Falcon 9 launch data from Wikipedia using BeautifulSoup
- Extracted and parsed HTML tables containing historical launch records
- Converted the scraped data into structured Pandas DataFrames for further processing

### 3. Exploratory Data Analysis (EDA) and Training Labels
- Performed exploratory data analysis using Matplotlib and Seaborn
- Analyzed relationships between payload mass, launch site, orbit type, booster version, and landing success
- Created and labeled the target variable required for machine learning classification

### 4. Database Integration and SQL Analysis
- Loaded the cleaned dataset into a Db2 database
- Executed SQL queries to:
  - Analyze landing outcomes
  - Identify trends over time
  - Compare success rates across launch sites and booster versions

### 5. Feature Engineering and Visualization
- Engineered new features to improve model performance
- Built interactive maps using Folium to visualize:
  - Launch site locations
  - Success and failure markers
  - Proximity to coastlines and nearby cities
- Identified geographic and operational patterns affecting landing success

### 6. Interactive Visual Analytics with Plotly Dash
- Developed an interactive Plotly Dash application
- Implemented dropdown menus and range sliders to dynamically explore:
  - Launch success rates
  - Payload mass distributions
  - Launch site performance
- Enabled real-time, user-driven visual analytics

### 7. Machine Learning Models and Hyperparameter Tuning
- Standardized the dataset and split it into training and test sets
- Trained multiple classification models:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - Decision Tree Classifier
- Tuned hyperparameters using GridSearchCV
- Evaluated models using accuracy scores and confusion matrices

---

## Results

- **Decision Tree Classifier** achieved the highest accuracy of about **89%**, making it the best-performing model
- **Support Vector Machine (SVM)** and **K-Nearest Neighbors (KNN)** each achieved an accuracy of about **84%**
- The results confirm that Falcon 9 landing success can be effectively predicted using historical launch data

---

## Conclusion

This project demonstrates that data-driven analytics and machine learning can successfully predict Falcon 9 first-stage landing outcomes.

Key factors influencing landing success include:
- Payload mass
- Launch site
- Orbit type
- Booster version
- Mission history

The insights gained from this analysis are valuable for:
- Estimating launch costs
- Understanding rocket reusability trends
- Supporting competitive decision-making in the commercial space industry

---

## Acknowledgments

- **IBM** — for providing the Applied Data Science Capstone curriculum  
- **Coursera** — for hosting the course and learning platform  
- **SpaceX** — for making launch data publicly available  

---

## Final Note

This repository presents a complete end-to-end data science workflow — from data collection and wrangling to visualization, modeling, and deployment.

It is intended for learners, professionals, and enthusiasts interested in applied data science, machine learning, and space analytics.

---

*This project was completed as part of the IBM Data Science Professional Certificate on Coursera.*
