# Forest Fire Risk Prediction

A machine learning project that predicts forest fire risk levels (Low, Medium, High) using environmental and weather data from the UCI Forest Fires dataset.


**Project Overview **
Forest fires are a major environmental concern, and early risk prediction can help prevent damage.
This project uses a Random Forest Classifier to classify fire risk categories based on features like temperature, humidity, wind, and drought indices.

Dataset

Source: UCI Machine Learning Repository – Forest Fires Dataset

Features:

Weather: temperature, wind, rain, relative humidity

Drought indices: DC, DMC, ISI, FFMC

Temporal: month, day (one-hot encoded)

Target: Burned area converted into risk levels:

Low (area ≤ 1)

Medium (1 < area ≤ 5)

High (area > 5)

Approach

Data Preprocessing

One-hot encoded month and day

Mapped burned area into 3 risk categories

Model Training

Random Forest Classifier

Train-test split for evaluation

Evaluation

Accuracy, precision, recall, F1-score

Confusion matrix to visualize predictions

Insights

Feature importance ranking to identify key predictors

Results

Accuracy: ~54% on test data

Class Performance:

Low risk: High recall (0.78)

Medium / High risk: Lower performance due to data imbalance

Most Important Features:

Temperature, Wind, DC, DMC, ISI indices

Visualizations Included:

Risk distribution plot

Confusion matrix

Feature importance chart

Future Improvements

Hyperparameter tuning using GridSearchCV

Handle class imbalance with SMOTE or weighted loss

Try advanced models (XGBoost, LightGBM)

Deploy as an interactive web app (Streamlit / Flask)

Author

Your Name – Your GitHub Profile
