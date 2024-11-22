# Falcon 9 Landing Success Prediction Project
This project analyzes SpaceX Falcon 9 launch data to predict the likelihood of a successful first-stage landing, a crucial step toward reducing space launch costs. By leveraging data collection, wrangling, exploratory data analysis (EDA), and predictive modeling, the project uncovers patterns and trends in launch outcomes.

![ibm1](https://github.com/user-attachments/assets/20e3d6b2-d80f-41cc-80e2-7e6d4e1cef36)

# Overview
![ibm6](https://github.com/user-attachments/assets/7a1e7bbe-7bfd-49b8-aa7e-07d3a7d2757f)

## Objective
Problem: Predict successful landings of Falcon 9's first stage to optimize launch cost estimations and improve competitive bidding.
Solution: Develop a data pipeline and predictive model using classification techniques.

## Results
Comprehensive interactive analytics and visualizations were created.
The Decision Tree model achieved the highest accuracy of 89%, making it the best model for predicting launch outcomes.


# Project Workflow
![ibm2](https://github.com/user-attachments/assets/731cb124-23a6-4fb6-b4df-b35c92ccdf05)
## 1. Data Collection
### Sources:

SpaceX REST API for detailed launch data.

Web scraping Falcon 9 launch records from Wikipedia.

Tools: requests, BeautifulSoup, pandas.

## 2. Data Wrangling
### Addressed missing values by:

Replacing nulls in numeric fields (e.g., PayloadMass) with the mean.

Retaining None for landing pad details where absent.

Preprocessed features for modeling.

## 3. Exploratory Data Analysis (EDA)
### Visualizations:

Scatter plots (e.g., Payload vs. Launch Site, Flight Number vs. Orbit Type).

Success rates per orbit type and payload range.

Yearly trends in launch success.

Tools: matplotlib, seaborn.

## 4. Interactive Visual Analytics
Built an interactive dashboard using Plotly Dash and Folium:

### Features:
Payload success vs. launch site analysis.

Filter options by site and payload range.

Markers indicating success (green) or failure (red).

## 5. Predictive Modeling
### Steps:

Feature extraction and standardization.

Train-test split.

Model evaluation and hyperparameter tuning using GridSearchCV.

### Models Used:

Logistic Regression.

Support Vector Machines (SVM).

Decision Trees (best performer).

K-Nearest Neighbors (KNN).

### Metrics: 
Accuracy scores and confusion matrices.

# Key Findings
![ibm3](https://github.com/user-attachments/assets/3db5c334-e368-47ab-a1f2-99f4ca27633f)

### Launch Sites:
Success rates are higher at specific sites (e.g., LEO orbit shows the highest success).

### Payload Trends:
Mid-range payloads (2000–5000 kg) have the highest success rates.

### Yearly Insights:
Significant improvement in success rates post-2013, stabilizing in 2017.

## Conclusion
![ibm4](https://github.com/user-attachments/assets/f2fdce40-ee4c-45c7-8dd7-8ff0904d276b)

### Impact: 
This project highlights critical factors driving launch success and provides actionable insights for SpaceX.

### Future Work: 
Expand the model to include more features like weather conditions and launch delays for even higher accuracy.

## Dependencies
Programming Language: ```python```

Libraries: ```pandas```, ```numpy```, ```matplotlib```, ```seaborn```, ```plotly```, ```scikit-learn```, ```Dash```, ```Folium```, ```BeautifulSoup```

## Acknowledgments
This project is based on the SpaceX dataset and uses publicly available APIs and web-scraped data. Special thanks to Coursera's Data Science Capstone Template.

![ibm5](https://github.com/user-attachments/assets/23259689-49fa-498e-afa9-c2d48c6b65a3)



