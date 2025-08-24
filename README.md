# Forest Fire Risk Prediction

A machine learning project that predicts forest fire risk levels (Low, Medium, High) using environmental and weather data from the UCI Forest Fires dataset.
Built with **Python**, **Pandas**, **Scikit-learn**, and **Matplotlib**.

---

## Overview

Forest fires are unpredictable and destructive.  
This project demonstrates how **machine learning** can classify **fire risk** from environmental conditions.  
We use the **UCI Forest Fires dataset**, preprocess it, train a **Random Forest Classifier**, evaluate its performance, and visualize the results.

---

## Dataset

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/forest+fires)  
- **Features:**
  - Weather: temperature, wind, humidity, rainfall  
  - Drought indices: DC, DMC, ISI, FFMC  
  - Temporal: month, day (one-hot encoded)  
- **Target variable:** Fire risk category (Low / Medium / High) derived from burned area

---

## Approach

1. **Data Preprocessing**  
   - One-hot encoding for `month` and `day`  
   - Converted burned area into risk categories  

2. **Model Training**  
   - Random Forest Classifier  
   - Train-test split evaluation  

3. **Evaluation**  
   - Accuracy, precision, recall, F1-score  
   - Confusion matrix visualization  

4. **Feature Insights**  
   - Ranked feature importances to identify key predictors  

---

## Results

- **Accuracy:** ~54%  
- **Class-wise performance:**
  - Low risk → High recall (0.78)  
  - Medium / High risk → Lower performance due to class imbalance  
- **Key features:** temperature, wind, DC, DMC, ISI  

### Visualizations included:
- Risk distribution plot  
- Confusion matrix heatmap  
- Feature importance bar chart  


---

## Future Improvements

- Hyperparameter tuning (GridSearchCV)  
- Handle class imbalance with SMOTE  
- Try gradient boosting (XGBoost / LightGBM)  
- Deploy as an interactive web app (Streamlit / Flask)  

---

