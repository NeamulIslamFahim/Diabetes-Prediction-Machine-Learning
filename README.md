# Diabetes Prediction Model

This project involves building a machine learning model to predict whether a person has diabetes based on several medical parameters. Various models are tested, and the best-performing model is selected based on accuracy.

## Dataset

The dataset used for this project contains several medical parameters of patients, which are used as features to predict whether the patient has diabetes or not.

### Features:
- Number of Pregnancies
- Glucose Level
- Blood Pressure
- Skin Thickness
- Insulin Level
- BMI (Body Mass Index)
- Diabetes Pedigree Function
- Age

### Target Variable:
- `y`: Whether the patient has diabetes (`1`) or not (`0`)

## Project Workflow

The workflow of this project can be summarized as follows:

1. **Data Exploration & Visualization**
   - Number of data points and target variable distribution.
   - Visualizing the feature space.

2. **Model Building**
   - Several machine learning models are evaluated, including:
     - Logistic Regression
     - Support Vector Machine (SVM)
     - Decision Tree Classifier
     - K-Nearest Neighbors (KNN)
     - Random Forest Classifier
     - Naive Bayes
     - Gradient Boosting
     - XGBoost

3. **Model Evaluation**
   - The models are evaluated based on their accuracy score.
   - A model comparison graph is plotted to show the accuracy of each model.

4. **Final Model Selection**
   - The model with the highest accuracy is selected as the final model.

## Files

- **target_distribution.png**: Distribution of the target variable (class distribution).
- **feature_space.png**: A 2D feature space plot (for simplicity, assuming 2D features).
- **model_comparison.png**: Comparison of the models based on their accuracy scores.

## Steps to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/diabetes-prediction.git
