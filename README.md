# Customer-Purchase-Prediction-on-Synthetic-E-Commerce-Data
This project focuses on predicting whether a customer will purchase a product using a synthetic e-commerce dataset. The dataset was initially unlabeled, and I applied manual labeling techniques based on behavioral thresholds. The objective was to build a classification model that can learn from user behavior and predict future purchases.

## Objectives
- Convert raw unlabeled data into a labeled classification dataset
- Detect and handle outliers and data quality issues
- Use both Scikit-learn and PyCaret to compare model performance
- Generate actionable insights from customer behavior patterns
  
## Technologies Used
- Python (Jupyter Notebook)
- Pandas, NumPy
- Scikit-learn
- PyCaret
- Matplotlib, Seaborn

## Project Pipeline
**1.Manual Labeling Logic**
- Used business-like thresholds (e.g., time on site, cart additions, bounce rate) to determine if a customer is likely to purchase
- Created a binary label: purchase = 1 or purchase = 0

**2.Data Preprocessing**
- Handled missing values and outliers using IQR and z-score techniques
- Encoded categorical variables (e.g., one-hot encoding)
- Normalized numerical features using StandardScaler

**3. Modeling Approaches**
- Scikit-learn: Implemented Logistic Regression, Random Forest, and Gradient Boosting with manual parameter tuning
- PyCaret: Used setup() and compare_models() for automated model comparison and evaluation

**4. Model Evaluation**
- Confusion matrix, ROC-AUC, Precision-Recall, and F1 Score
- Compared manual and automated pipelines for performance

## Results
- Best-performing model: [DT, Bagging, AdaBoost, GDBoost, XGBoost]
- Achieved over 85% accuracy in predicting purchases
- Key features influencing purchase: session duration, number of product views, cart activity

## Business Impact
- Helps simulate a real-world product recommendation engine
- Manual labeling approach mimics real data curation efforts in industry
- Provides a pipeline for marketing and product teams to target potential buyers
