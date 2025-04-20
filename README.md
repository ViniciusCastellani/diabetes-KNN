# README - Diabetes Risk Prediction using KNN Clustering

## Project Overview
This Python project analyzes the Pima Indians Diabetes dataset to predict diabetes risk based on glucose levels and BMI (Body Mass Index) using K-Nearest Neighbors (KNN) clustering and classification.

## Dataset Source
- **Dataset**: Pima Indians Diabetes Database
- **Source**: [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Features Used**: Glucose, BMI, and Outcome (diabetes indicator)

## Key Features
1. **Data Analysis**:
   - Correlation analysis between features
   - Data normalization using MinMaxScaler
   - Separation of data into diabetic and non-diabetic groups

2. **Clustering**:
   - KNN-based clustering of patients
   - Automatic cluster formation based on glucose and BMI
   - Centroid calculation for each cluster
   - Cluster visualization with meaningful health interpretations

3. **Prediction Model**:
   - KNN Regressor for diabetes risk prediction
   - Interactive console interface for user input
   - Binary classification (diabetic/non-diabetic)

## Requirements
- Python 3.x
- Required libraries:
  ```bash
  pip install numpy pandas scikit-learn matplotlib
  ```

## How to Use
1. **Data Preparation**:
   - Place `diabetes.csv` in the same directory as the script
   - The script automatically loads and preprocesses the data

2. **Visualization**:
   - The script generates two main visualizations:
     - Cluster plot for non-diabetic patients
     - Cluster plot for diabetic patients
   - Each cluster includes health interpretations for glucose levels and BMI

3. **Prediction**:
   - Run the script and use the interactive prompt:
     ```
     Informe seu nível de Glucose: [value]
     Informe seu BMI (Índice de Massa Corporal): [value]
     ```
   - The model will predict diabetes risk based on input values

## Code Structure
1. **Data Loading & Preprocessing**:
   - Loads diabetes dataset
   - Checks for missing values
   - Selects relevant features (Glucose and BMI)

2. **Clustering**:
   - Normalizes data
   - Calculates nearest neighbors
   - Forms clusters based on distance thresholds
   - Computes cluster centroids and radii

3. **Visualization**:
   - Creates scatter plots with cluster circles
   - Adds health interpretations for each cluster
   - Color-codes different clusters

4. **Prediction Model**:
   - Trains KNN regressor
   - Provides interactive prediction interface
   - Outputs diabetes risk assessment

## Interpretation
- **Glucose Levels**:
  - Very high (≥0.90 normalized)
  - High (0.75-0.90)
  - Moderate (0.55-0.75)
  - Normal (0.40-0.55)
  - Low (<0.40)

- **BMI Categories**:
  - Obesity grade III (≥0.80)
  - Obesity grade II (0.70-0.80)
  - Obesity grade I (0.60-0.70)
  - Overweight (0.50-0.60)
  - Normal weight (0.40-0.50)
  - Underweight (<0.40)

## Results
The project provides:
1. Visual cluster analysis of diabetic vs non-diabetic patients
2. Interactive diabetes risk prediction
3. Health interpretations for each cluster based on glucose and BMI levels
