# 📊 Customer Churn Prediction (Telco Dataset)

## 📌 Project Overview

This project focuses on predicting customer churn using machine learning techniques on a real-world telecom dataset. The goal is to identify customers who are likely to leave the service so that businesses can take proactive retention measures.

The dataset used is the **Telco Customer Churn dataset**, which contains customer demographics, account information, and service usage details.

---

## 📂 Dataset

* Source: Telco Customer Churn Dataset
* File used: `WA_Fn-UseC_-Telco-Customer-Churn.csv`
* Contains information such as:

  * Customer demographics
  * Services subscribed
  * Billing information
  * Churn status

---

## ⚙️ Project Workflow

### 1. Data Loading

* Loaded dataset using **Pandas**
* Inspected structure using `.head()` and `.info()`

### 2. Data Preprocessing

* Converted `TotalCharges` to numeric format
* Handled missing values using **median imputation**
* Encoded target variable (`Churn`) using **LabelEncoder**
* Applied **One-Hot Encoding** (`get_dummies`) for categorical features

---

### 3. Exploratory Data Analysis (EDA)

* Used **Seaborn** and **Matplotlib** for visualization
* Analyzed:

  * Churn distribution
  * Feature relationships
  * Correlation patterns

---

### 4. Feature Scaling

* Applied **StandardScaler** to normalize numerical features
* Ensured better performance for distance-based models

---

### 5. Model Training

The following machine learning models were implemented:

* 🌳 Random Forest Classifier
* 📍 K-Nearest Neighbors (KNN)
* 📊 Gaussian Naive Bayes

---

### 6. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC Curve & AUC Score

---

## 📈 Results & Insights

* Compared performance of multiple models
* Identified the most effective model for churn prediction
* Found important features influencing churn using **feature importance (Random Forest)**

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📁 File Structure

```
Customer_Churn_Project.ipynb   # Main notebook
README.md                      # Project documentation
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/AnshSingh109/Customer_Churn_Prediction_Project.git
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## 💡 Future Improvements

* Hyperparameter tuning using GridSearchCV
* Try advanced models (XGBoost, LightGBM)
* Deploy using Flask/Django
* Build a dashboard for visualization

---

## 🤝 Contributing

Feel free to fork this repository and improve the project.

---

## 📜 License

This project is open-source and available under the MIT License.
