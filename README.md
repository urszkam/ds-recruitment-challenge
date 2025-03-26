# 🚗 Car Price Prediction – Kaggle Competition

## Project Overview

This project aims to build a predictive model capable of accurately estimating car prices based on detailed listings scraped from a popular classified ads website. The dataset includes extensive vehicle information such as brand, model, production year, mileage, fuel type, and equipment features.

📂 The dataset consists of the following files:

- `sales_ads_train.csv` – Original training data with vehicle prices.
- `synthetic_training_data_sdv_pl.csv` – Synthetic data generated using the SDV framework.
- `synthetic_training_data_mostlyai_pl.csv` – Synthetic data generated using the MostlyAI platform.
- `sales_ads_test.csv` – Test data without prices, used for model evaluation.

## Project Tasks

<div style="display: flex; align-items: flex-start;">
  <div style="flex: 1; padding-right: 20px;">
    <p>- **Exploratory Data Analysis (EDA)**: We conducted an in-depth analysis of both numerical and categorical features to understand distributions, identify outliers, and assess missing values. The EDA helped us uncover key patterns and relationships influencing car prices.</p>
  </div>
  <div style="flex: 1;">
    <img src="image.png" alt="EDA Visualization" style="max-width: 100%;">
  </div>
</div>
- **Data Preprocessing and Feature Engineering**: We cleaned and preprocessed the dataset by handling missing values, transforming variables (e.g., converting complex features like equipment lists into usable formats), and filling most missing values based on the most frequent values observed in brand:model pairs.
- **Model Training and Tuning**: We initially conducted traditional regression analysis, followed by neural network modeling using Keras. Our final predictive model was built using AutoGluon to automatically optimize performance and effectively capture the factors driving car prices.
- **Kaggle Competition Submission**: We prepared and submitted our predictions for evaluation on Kaggle, incorporating cross-validation and ensemble strategies to improve accuracy.


## Technologies and Libraries

The project utilizes the following Python libraries:
- **Jupyter Notebook** – interactive development and documentation environment
- **NumPy** – numerical computations and array operations
- **Pandas** – data manipulation and analysis
- **Scikit-learn** – Data preprocessing and modeling
- **Seaborn** – Visualization and exploratory analysis
- **Matplotlib** – comprehensive library for creating static, animated, and interactive visualizations
- **AutoGluon** – automated machine learning toolkit for rapidly building accurate models

## Evaluation Metrics

Model performance was evaluated using the following metrics:
- **R-squared (R²)** – to measure the proportion of variance in the car prices explained by our model.
- **Root Mean Squared Error (RMSE)** – the primary evaluation metric on Kaggle, assessing the average prediction error in the same units as the target variable.
