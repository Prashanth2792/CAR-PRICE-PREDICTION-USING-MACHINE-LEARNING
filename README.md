# 🚗 Car Price Prediction Using Machine Learning

## 📌 Project Overview

The **Car Price Prediction Using Machine Learning** project aims to predict the estimated selling price of used cars based on important vehicle features such as brand, manufacturing year, kilometers driven, fuel type, seller type, transmission, and ownership history.

This project follows an end-to-end Machine Learning workflow, starting from data collection and exploratory data analysis (EDA) to model development, evaluation, model saving, and interactive deployment using Gradio.

## 🎯 Problem Statement

Estimating the resale value of a used car can be challenging because its price depends on several factors, including vehicle age, brand, usage, fuel type, and condition.

The objective of this project is to build a regression-based Machine Learning model that learns patterns from historical car data and predicts an estimated selling price based on user-provided vehicle details.

## 🎯 Project Objectives

- Understand and analyze the used-car dataset.
- Perform data cleaning and preprocessing.
- Explore relationships between vehicle features and selling prices.
- Apply feature engineering to extract useful information.
- Train and compare multiple regression algorithms.
- Evaluate models using appropriate regression metrics.
- Save the best-performing Machine Learning pipeline.
- Develop an interactive prediction interface using Gradio.

## 📂 Dataset Description

The project uses a CarDekho used-car dataset.

**Original dataset dimensions:**
- Rows: 4,340
- Columns: 8

**Dataset features:**

| Feature | Description |
|---|---|
| `name` | Car name and model |
| `year` | Manufacturing year |
| `selling_price` | Selling price of the car (target variable) |
| `km_driven` | Total kilometers driven |
| `fuel` | Fuel type |
| `seller_type` | Type of seller |
| `transmission` | Manual or automatic |
| `owner` | Previous ownership details |

**Data cleaning:** 763 duplicate records were identified and removed, resulting in a cleaned dataset containing **3,577 rows and 8 columns**.

## 🔍 Project Workflow

1. **Business Understanding:** Defined the problem and prediction objective.
2. **Data Collection:** Loaded the CarDekho dataset.
3. **Data Understanding:** Examined dataset structure, data types, and statistical summaries.
4. **Data Cleaning:** Identified and removed duplicate records.
5. **Exploratory Data Analysis:** Analyzed distributions, relationships, and patterns using visualizations.
6. **Feature Engineering:** Extracted the car brand from the car name.
7. **Data Preprocessing:** Applied numerical imputation and One-Hot Encoding for categorical features.
8. **Train-Test Split:** Divided the data into 80% training and 20% testing sets.
9. **Model Building:** Trained multiple regression algorithms.
10. **Model Evaluation:** Compared model performance using MAE, RMSE, and R².
11. **Model Saving:** Saved the selected Machine Learning pipeline using Joblib.
12. **Deployment:** Created an interactive prediction interface using Gradio in Jupyter Notebook.

## 📊 Exploratory Data Analysis (EDA)

EDA was performed to understand the dataset and identify patterns affecting used-car prices.

Key analysis included:

- Distribution of selling prices.
- Relationship between manufacturing year and selling price.
- Relationship between kilometers driven and selling price.
- Selling-price comparison across fuel types.
- Analysis of categorical feature distributions.
- Correlation analysis of numerical features.

## 🤖 Machine Learning Models

The following regression algorithms were implemented and compared:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

### 📈 Model Evaluation Results

The models were evaluated on the test dataset using three regression metrics.

| Model | MAE (₹) | RMSE (₹) | R² Score |
|---|---:|---:|---:|
| Random Forest | 156,498.17 | 359,335.07 | 0.599 |
| Decision Tree | 185,480.05 | 398,804.80 | 0.506 |
| Linear Regression | 206,368.40 | 431,734.10 | 0.421 |

### 🏆 Best Model: Random Forest Regressor

Random Forest achieved the best performance among the three models in this experiment, with the lowest MAE and RMSE and the highest R² score.

**Best model performance:**
- MAE: ₹1,56,498.17
- RMSE: ₹3,59,335.07
- R² Score: 0.5992

The R² score indicates that the model explains approximately 59.92% of the variation in selling prices on the test dataset. It does not represent prediction accuracy.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Development Environment:** Jupyter Notebook
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Model Serialization:** Joblib
- **Interactive Deployment:** Gradio

## 📁 Project Structure

```text
ML_Project/
│
├── dataset/
│   └── car data.csv
│
├── notebooks/
│   └── car_price_prediction.ipynb
│
├── models/
│   └── car_price_model.pkl
│
├── README.md
├── requirements.txt
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

### 2. Navigate to the Project Folder

```bash
cd ML_Individual_Project
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the Project

Open the `car_price_prediction.ipynb` notebook and execute the cells in sequence.

## 🌐 Gradio Application

An interactive application was developed using Gradio to allow users to enter vehicle details and receive an estimated selling price.

**User inputs include:**
- Car brand
- Manufacturing year
- Kilometers driven
- Fuel type
- Seller type
- Transmission type
- Ownership details

The application passes these inputs to the saved Machine Learning pipeline and displays the predicted car selling price.

**To launch:** Run the Gradio interface cells in the Jupyter Notebook.

## ⚠️ Limitations

- The model's performance depends on the quality and coverage of the dataset.
- The dataset may not represent current market prices.
- Some important factors, such as vehicle condition, location, service history, and accident history, are not included.
- The current R² score indicates scope for further improvement.
- Predictions should be treated as estimates, not guaranteed market prices.

## 🚀 Future Improvements

- Perform hyperparameter tuning to improve model performance.
- Include additional vehicle features.
- Explore advanced regression algorithms.
- Improve feature engineering.
- Use updated datasets to reflect current market conditions.
- Improve the Gradio interface and deployment process.

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Understanding real-world Machine Learning problems.
- Performing data cleaning and EDA.
- Preparing numerical and categorical features.
- Building Scikit-learn preprocessing pipelines.
- Training and evaluating regression models.
- Comparing model performance using evaluation metrics.
- Saving and reusing trained Machine Learning models.
- Developing an interactive ML application using Gradio.

## 👨‍💻 Author

**Kota Prashanth Yadav**

B.Tech – Data Science | 2026 Graduate

Interested in Data Science, Machine Learning, Python, and Data Analytics.

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback!
