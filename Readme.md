#  Laptop Price Prediction using Machine Learning

##  Project Overview
This project focuses on building a machine learning model to predict laptop prices based on their technical specifications such as brand, processor, RAM, storage, and weight.

The goal is to demonstrate an **end-to-end machine learning workflow**, covering data preprocessing, model training, hyperparameter tuning, evaluation, and real-time prediction using user input.

---

##  Problem Statement
Laptop prices vary significantly depending on hardware configuration and brand.  
Accurately predicting laptop prices can help:
- Customers make informed purchasing decisions  
- Businesses price products competitively  

This project aims to predict laptop prices using supervised regression techniques.

---

## Tools & Technologies
- Python  
- Jupyter Notebook  
- Pandas, NumPy  
- Scikit-learn  
- Machine Learning (Regression & Ensemble Models)

---

##  Dataset Description
The dataset contains information about laptops, including:
- Brand  
- Processor type  
- RAM size  
- Storage capacity  
- Operating system  
- Weight  
- Price (target variable)

The target variable is **Laptop Price**.

---

##  Exploratory Data Analysis (EDA)
- Analyzed data structure and feature distributions  
- Identified numerical and categorical variables  
- Observed price variation across different hardware configurations  
- Checked and handled missing values  

EDA helped understand key factors influencing laptop prices.

---

## Feature Engineering & Preprocessing
- Encoded categorical variables into numerical format  
- Handled missing values using median imputation (to avoid data leakage)  
- Split the dataset into training and testing sets  
- Prepared the data for regression-based machine learning models  

---

##  Model Training & Optimization
The following models were trained and evaluated:

### Random Forest Regressor
- Used as a baseline ensemble model  
- Captures non-linear relationships between features  

###  Hyperparameter Tuning (Random Forest)
- Optimized parameters such as number of trees and depth  
- Improved model performance and generalization  

###  Gradient Boosting Regressor
- Advanced ensemble model that builds trees sequentially  
- Effectively reduces bias and captures complex patterns  

###  Hyperparameter Tuning (Gradient Boosting)
- Tuned learning rate, number of estimators, and depth  
- Achieved the best overall performance  

---

##  Model Evaluation
Models were evaluated using:
- **R² Score**  
- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**  

After comparison, the **tuned Gradient Boosting Regressor** was selected as the final model due to superior predictive performance.

---

##  User Input-Based Prediction
The notebook includes a user input section where users can enter laptop specifications to receive a predicted price.

This demonstrates how the trained model can be used in a real-world scenario for price estimation.

> Note: In a production environment, this logic would be implemented through a web application or API.

---

## Conclusion
This project demonstrates a complete machine learning pipeline:
- Data exploration and preprocessing  
- Model training and hyperparameter tuning  
- Performance evaluation  
- Practical prediction using user input  

The final model effectively captures the relationship between laptop specifications and price.

---

##  Future Improvements
- Add GPU, screen resolution, and brand popularity features  
- Apply cross-validation for more robust evaluation  
- Deploy the model using Flask or FastAPI  
- Integrate the model into a web-based application  

---

##  Files in This Repository
- `Laptop_Price_Prediction.ipynb` – Jupyter Notebook with full implementation  
- `data/` – Dataset used for training (if included)  


