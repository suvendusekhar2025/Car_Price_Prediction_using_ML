# Car_Price_Prediction_using_ML
Here’s a well-structured and detailed project description for the **Car Price Prediction using Machine Learning** project:

---

### **Project Title:** Car Price Prediction using Machine Learning

### **Project Description:**

This project focuses on building a machine learning model to predict car prices based on various features using a dataset containing information on used cars. The dataset used is in CSV format, consisting of **301 rows and 9 columns**, with each row representing a car and its associated features such as year, present price, kilometers driven, fuel type, seller type, transmission type, and ownership.

### **Technologies and Libraries Used:**

- **Python**
- **Libraries:**  
  - **NumPy** – for numerical operations  
  - **Pandas** – for data manipulation and analysis  
  - **Matplotlib** and **Seaborn** – for data visualization  
  - **Scikit-learn (sklearn)** – for model selection and evaluation  

### **Data Preprocessing:**

1. **Handling Categorical Variables:**
   - The dataset contains categorical features such as 'fuel_type`, `seller_type`, & `transmission`.
   - These columns were **converted to numerical values** using **Label Encoding**:
     - For example:  
       'fuel_type`: Petrol → 0, Diesel → 1, CNG → 2, etc.

2. **Splitting the Dataset:**
   - The dataset was split into **training** and **testing sets** using **train_test_split** from `sklearn.model_selection` to evaluate model performance effectively.

### **Modeling Approach:**

Two regression models were implemented and compared:

1. **Linear Regression**
2. **Lasso Regression** (L1 Regularization)

Both models were trained on the training set and evaluated on the test set using the **R² Score (R-squared error)** from `sklearn.metrics`, since the target variable (car price) is continuous.

#### **Model Performance:**

| Model             | Training R² Score | Testing R² Score |
|------------------|-------------------|------------------|
| Linear Regression | 87.99%            | 83.65%           |
| Lasso Regression  | 84.27%            | 87.09%           |

- The **Lasso Regression model** slightly outperformed Linear Regression on the test data, indicating better generalization and reduced overfitting.

### **Visualization:**

- A **scatter plot** was created using **Matplotlib** to visualize the comparison between **actual car prices** and **predicted car prices**.
- This plot helped to identify the closeness of predicted values to the actual prices and understand the model’s performance visually.

---
