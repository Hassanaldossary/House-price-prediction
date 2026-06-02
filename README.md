# House Price Prediction Using Machine Learning

## Project Overview

This project develops and evaluates machine learning models for predicting residential property prices based on property characteristics, location, and amenities. The objective is to build accurate predictive models while demonstrating a complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation.

---

## Problem Statement

Accurate house price estimation is essential for buyers, sellers, investors, and real estate companies. Traditional pricing methods often rely on manual assessment and market expertise, while machine learning models can leverage historical data to identify complex patterns and provide data-driven price predictions.

---

## Dataset

The dataset contains information about residential properties and their selling prices.

### Features

#### Numerical Features

* BHK
* Bathrooms
* Super Area (SqFt)
* Carpet Area (SqFt)
* Floor Number
* Total Floors
* Property Age
* Parking Spaces
* Distance to Metro (km)
* Distance to City Center (km)

#### Categorical Features

* City
* Property Type
* Furnishing Status
* Locality Type

### Target Variable

* House Price (INR Lakhs)

The dataset is included in the repository under the `data/` directory.

---

## Project Workflow

### 1. Data Cleaning

* Removed duplicate records
* Handled missing values
* Validated feature consistency

### 2. Exploratory Data Analysis (EDA)

* Distribution analysis
* Correlation analysis
* Outlier detection using boxplots
* Feature-target relationship analysis

### 3. Feature Engineering

* One-Hot Encoding for nominal categorical variables
* Ordinal Encoding for ordered categorical variables
* Feature transformation using Scikit-Learn pipelines

### 4. Model Development

The following machine learning models were implemented and compared:

* Linear Regression
* Random Forest Regressor
* XGBoost Regressor

### 5. Model Evaluation

Models were evaluated using:

* R² Score
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* 5-Fold Cross Validation

---

## Results

| Model                   | R² Score | RMSE |
| ----------------------- | -------- | ---- |
| Linear Regression       | 0.65     | 87   |
| Random Forest Regressor | 0.78     | 68   |
| XGBoost Regressor       | 0.77     | 70   |

Random Forest achieved the best overall performance and demonstrated a stronger ability to capture non-linear relationships between property characteristics and housing prices.

---

## Key Findings

* Property size is one of the strongest predictors of house price.
* Location significantly influences property valuation.
* Premium localities generally command higher prices.
* Ensemble methods outperform Linear Regression due to their ability to model complex, non-linear relationships.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* Jupyter Notebook

---

## Repository Structure

```text
House-Price-Prediction/
│
├── data/
├── notebooks/
├── images/
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd House-Price-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

---

## Future Improvements

* Hyperparameter optimization
* Additional feature engineering
* Model deployment using Flask or FastAPI
* Integration with a web-based user interface
* Exploration of deep learning approaches

---

## Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Data Preprocessing
* Machine Learning Pipelines
* Regression Modeling
* Cross Validation
* Model Evaluation
* Ensemble Learning

---

## Author

**Hassan Aldossari**

Computer Science Student at KFUPM
Aspiring Machine Learning Engineer
