This project focuses on predicting patient readmissions within 30 days of discharge using the **Diabetes 130-US Hospitals Dataset**. The goal is to identify high-risk patients and provide actionable insights to healthcare providers to improve patient outcomes and reduce costs.

**Key Steps:**

1. **Data Preprocessing:**
* Handled missing values (represented by ?) by dropping irrelevant columns and rows.
* Converted the target variable (readmitted) into a binary classification problem (1 for readmission within 30 days, 0 otherwise).
* Encoded categorical variables using one-hot encoding.
* Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique).
2. **Model Building & Comparison:**
* Trained an XGBoost model and a Random Forest model to predict patient readmissions.
* Evaluated the models using ROC-AUC score, precision, recall, and F1-score.
3. **Compared the performance of both models:**
      * **XGBoost:** ROC-AUC = 0.891606, F1-score = 0.897196.
      * **Random Forest:** ROC-AUC = 0.932422, F1-score = 0.932039.
**Results:**
  
* Identified the top 10 features driving readmissions, including:
      * num_inpatient: Number of inpatient visits.
      * num_medications: Number of medications prescribed.
      * age: Patient age group.
* Visualized the models’ performance using **confusion matrices** and **feature importance plots.**
* **Tools & Technologies:**
   * Python Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn.
   * Techniques: Data cleaning, feature engineering, SMOTE, XGBoost, Random Forest, ROC-AUC analysis.

## How to Use This Repository
1. Clone the repository:
   ```bash
   git clone https://github.com/kileighboggess/predictive-modeling-readmissions.git

   pip install -r requirements.txt
