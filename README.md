# Student Performance Prediction

## Project Overview

This project aims to predict students' math scores using various machine learning algorithms. The analysis explores how student performance is affected by different variables such as gender, ethnicity, parental education level, lunch type, and test preparation.

## Dataset

The project uses the "Students Performance" dataset, which contains information about 1000 students with the following features:

- **gender**: Student gender (male/female)
- **race/ethnicity**: Racial/ethnic group (5 groups labeled A-E)
- **parental level of education**: Parents' highest education level (6 categories)
- **lunch**: Type of lunch received (standard/free/reduced)
- **test preparation course**: Whether the student completed a test preparation course (none/completed)
- **math score**: Math test score (0-100)
- **reading score**: Reading test score (0-100)
- **writing score**: Writing test score (0-100)

Dataset size: 1000 records with 8 columns (5 categorical features and 3 numerical features)

## Methodology

### Data Preprocessing

1. **Exploratory Data Analysis (EDA)**:

   - Analyzed the distribution of scores by gender, parental education, and lunch type
   - Created visualizations of feature relationships
   - Generated statistical summaries of the data
   - Identified no missing values in the dataset
2. **Feature Engineering**:

   - Created total score and average score features
   - Split the data into training (80%) and testing (20%) sets
   - One-hot encoded categorical variables
   - Standardized numerical features

### Machine Learning Models

The project evaluated multiple regression models:

1. **Linear Regression Models**:

   - Simple Linear Regression
   - Ridge Regression
   - Lasso Regression

2. **Tree-Based Models**:

   - Decision Tree
   - Random Forest

### Model Evaluation

Models were evaluated using:

1. R-squared (R²) score
2. Mean Absolute Error (MAE)
3. Mean Squared Error (MSE)
4. Root Mean Squared Error (RMSE)
5. 10-fold cross-validation

## Key Findings

- Ridge Regression and Linear Regression performed best with test R² scores around 0.88
- Parental education level and reading/writing scores were the most important predictors of math performance
- Female students generally outperformed male students
- Students with standard lunches performed better than those with free/reduced lunches
- Students who completed test preparation courses showed better performance

## Model Performance (Test R² scores)

- Ridge Regression: 0.880
- Linear Regression: 0.880
- Random Forest: 0.849
- Lasso Regression: 0.825
- Decision Tree: 0.731
