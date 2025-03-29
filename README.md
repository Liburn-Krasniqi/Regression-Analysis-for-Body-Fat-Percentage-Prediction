# Body Fat Percentage Estimation Project

![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)

## Project Description
This project aims to estimate **body fat percentage (BF%)** using easily measurable physical indicators such as age, weight, height, and various body circumference measurements. The analysis focuses on developing a predictive regression model to accurately estimate BF% from these measurements.

## Key Research Questions
1. Which indicators provide a reliable estimation of BF%?
2. What is the best regression model for predicting BF%?
3. How do individual variables contribute to the model's accuracy?

## Dataset
The dataset contains pre-recorded measurements of body fat percentage along with various physical indicators. The data was cleaned and preprocessed to handle outliers and unit inconsistencies.

### Data Cleaning Steps:
- Removed samples with physiologically impossible BF% values (<5%)
- Corrected unit inconsistencies (converted imperial to metric)
- Handled outliers using box plot analysis

## Methodology
1. **Exploratory Data Analysis (EDA)**
   - Visualized relationships between variables
   - Detected and handled outliers
   - Standardized the data for better model performance

2. **Feature Selection**
   - Tested individual features for correlation with BF%
   - Automated feature combination testing to find the optimal set

3. **Model Building**
   - Linear Regression (Best model: R² = 0.659)
   - Principal Component Analysis (PCA)
   - Random Forest Regressor
   - Ridge Regression

## Results
The best-performing model used the following features:
- Age
- Neck circumference
- Chest circumference
- Abdomen circumference
- Forearm circumference
- Wrist circumference
- BMI

### Performance Metrics:
- **R² Score:** 0.659
- **Mean Absolute Error:**  3.555727076353437
- **Root Mean Squared Error:** 4.399275287063576

## How to Use
1. Open the notebook in Google Colab using the badge above
2. Mount your Google Drive to access the dataset
3. Run the cells sequentially to:
   - Load and preprocess the data
   - Perform EDA
   - Train and evaluate models

## Dependencies
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - statsmodels

## Files
- `Project_A_ICT_AI_v_2.ipynb`: Main Jupyter notebook containing the analysis
- `PercentBodyFat.xlsx`: Dataset file
- `model.joblib`: Saved best model

## Author
Liburn Krasniqi
