#  Laptop Price Prediction Using Machine Learning

##  Project Summary

Laptop prices depend on multiple hardware features such as processor type, RAM size, storage capacity, display quality, and brand reputation. Understanding how these specifications influence price can help businesses build competitive pricing strategies and assist consumers in selecting laptops that match their needs and budgets.

This project builds a **machine learning regression model** to predict laptop prices using hardware specifications and engineered features derived from the dataset.

The project follows a complete **end-to-end machine learning workflow**, including data cleaning, exploratory analysis, feature engineering, model training, and evaluation.

---

#  Project Metrics

| Metric                | Value                       |
| --------------------- | --------------------------- |
| Dataset Size          | 1,273 laptops               |
| Original Features     | 11                          |
| Engineered Features   | 5+                          |
| Machine Learning Task | Regression                  |
| Libraries Used        | Pandas, NumPy, Scikit-Learn |

---

#  Dataset Overview

The dataset contains specifications for multiple laptop brands and configurations.

| Feature          | Description                                         |
| ---------------- | --------------------------------------------------- |
| Company          | Laptop brand (Dell, HP, Apple, Lenovo, etc.)        |
| TypeName         | Laptop category (Gaming, Notebook, Ultrabook, etc.) |
| CPU              | Processor model                                     |
| RAM              | Memory size                                         |
| Storage          | HDD / SSD configuration                             |
| GPU              | Graphics processor                                  |
| Operating System | Installed OS                                        |
| Weight           | Laptop weight                                       |
| Display          | Screen size and resolution                          |
| Price            | Target variable                                     |

After preprocessing, the dataset contains **1,273 usable laptop records** with multiple hardware features used for prediction.

---

#  Tools & Technologies

### Programming Language

* Python

### Libraries Used

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

### Techniques Applied

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Correlation Analysis
* Regression Modeling
* Model Evaluation

---

#  Data Preprocessing

The raw dataset required several preprocessing steps before training the model.

### Missing Value Handling

Rows containing null values were removed to maintain data consistency.

### Data Cleaning

Several columns contained text-based values such as:

```
8GB RAM
1.37kg weight
256GB SSD
```

These values were converted into **numeric features** for machine learning.

### Column Transformation

Unnecessary columns and duplicate indexing columns were removed to simplify the dataset.

---

# Feature Engineering

Feature engineering played a critical role in improving the predictive power of the model.

### 1️⃣ Touchscreen Feature

A new binary feature was created to identify laptops that support touchscreen displays.

| Touchscreen | Meaning                |
| ----------- | ---------------------- |
| 1           | Touchscreen laptop     |
| 0           | Non-touchscreen laptop |

Touchscreen laptops tend to have **higher prices**.

---

### 2️⃣ IPS Panel Feature

Display specifications were analyzed to determine whether the laptop includes an **IPS display panel**.

IPS displays generally provide **better color accuracy and viewing angles**, leading to higher prices.

---

### 3️⃣ Display Pixel Density

Screen resolution and screen size were combined to calculate **display pixel density (PPI)**.

```
Display = sqrt(width² + height²) / screen_size
```

This provides a better representation of display quality.

---

### 4️⃣ CPU Categorization

Processor models were grouped into major categories:

| CPU Category           |
| ---------------------- |
| Intel Core i3          |
| Intel Core i5          |
| Intel Core i7          |
| Other Intel Processors |
| AMD Processors         |

This transformation reduces feature complexity while preserving meaningful information.

---

#  Exploratory Data Analysis

Exploratory analysis revealed several interesting patterns.

---

## 🏷 Brand vs Laptop Price

Brands such as **Apple and Razer** consistently show higher average laptop prices.

Major laptop brands in the dataset include:

* Lenovo
* Dell
* HP
* Asus
* Apple

These brands also dominate the dataset in terms of product availability.

---

##  Laptop Type vs Price

Laptop categories show significant variation in pricing.

| Laptop Type | Pricing Trend                |
| ----------- | ---------------------------- |
| Notebook    | Most common, moderate price  |
| Ultrabook   | Premium pricing              |
| Gaming      | High performance, high price |
| Workstation | Very high price              |

---

##  RAM vs Price

RAM size has one of the strongest correlations with laptop price.

Higher RAM configurations significantly increase laptop prices.

---

## Display Features vs Price

Display features also influence laptop pricing.

Laptops with:

* Touchscreen displays
* IPS panels
* High-resolution screens

generally have **higher market prices**.

---

#  Machine Learning Model

The project uses **regression-based machine learning models** to predict laptop prices.

### Modeling Workflow

1. Data preprocessing and feature transformation
2. Feature selection
3. Train-test data split
4. Model training
5. Model evaluation

The trained model learns the relationship between laptop hardware specifications and market prices.

---

#  Model Evaluation

Model performance was evaluated using standard regression metrics.

| Metric   | Purpose                  |
| -------- | ------------------------ |
| MAE      | Average prediction error |
| MSE      | Penalizes larger errors  |
| R² Score | Measures model accuracy  |

These metrics help determine how well the model predicts laptop prices.

---

# 🔍 Key Insights

From the analysis, several key insights were discovered.

### RAM is the strongest price driver

Higher RAM configurations significantly increase laptop prices.

### Premium brands charge higher prices

Apple and Razer laptops appear consistently in the high-price range.

### Display quality impacts pricing

High-resolution displays and IPS panels increase laptop value.

### Gaming laptops are expensive

Gaming and workstation laptops contain high-performance hardware, leading to higher prices.

---

#  Business Applications

Laptop price prediction models have several real-world applications.

* E-commerce price recommendation systems
* Retail product pricing strategies
* Laptop price comparison tools
* Market trend analysis

---

#  Skills Demonstrated

This project highlights the following data science skills:

* Data Cleaning and Transformation
* Feature Engineering
* Exploratory Data Analysis
* Data Visualization
* Machine Learning Modeling
* Regression Analysis
* Business Insight Generation

---

#  Future Improvements

Possible future enhancements include:

* Deploying the model as a **web application**
* Creating an **interactive laptop price prediction tool**
* Training advanced regression models
* Integrating **real-time pricing datasets**

---

#  Conclusion

This project demonstrates how machine learning can be applied to analyze laptop specifications and predict their market prices.

By combining data preprocessing, feature engineering, exploratory analysis, and regression modeling, the project provides valuable insights into how different hardware components influence laptop pricing.
