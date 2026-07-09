# Diabetes Prediction System

A machine learning model that analyzes clinical health data — including Glucose, BMI, and Age — to predict the likelihood of diabetes with **80% accuracy**, offering data-driven medical insights.

🔗 **Live Demo:** [https://hadiaahmed.pythonanywhere.com/](https://hadiaahmed.pythonanywhere.com/)

## Introduction

**Definition:** A binary classification ML task that predicts whether a patient is Diabetic (1) or Non-Diabetic (0) using clinical health attributes such as Glucose level, BMI, Insulin, Age, and Blood Pressure.

**Application:** Used in healthcare analytics for early disease detection, testing machine learning algorithms on medical datasets, and gaining insights into how physiological factors contribute to diabetic risk.

## Input Features

| Feature | Possible Values |
|---|---|
| Pregnancies | 0 to 17 (Number of times pregnant) |
| Glucose | 0 to 200 (Plasma glucose concentration) |
| BloodPressure | 0 to 122 (Diastolic blood pressure) |
| SkinThickness | 0 to 99 (Triceps skin fold thickness) |
| Insulin | 0 to 846 (2-Hour serum insulin) |
| BMI | 0.0 to 67.1 (Body Mass Index) |
| Pedigree | 0.08 to 2.42 (Genetic risk score) |
| Age | 21 to 81 (Years) |

## Output

| Output Attribute | Possible Values |
|---|---|
| Diabetic | Yes, No |

## How It Works

1. **Load & Explore Data** — Reads the sample dataset (`diabetes_data.csv`) into a pandas DataFrame.
2. **Preprocessing** — Dataset is already clean and numerical, so no additional preprocessing or feature extraction is required.
3. **Train/Test Split** — Splits data into 80% training and 20% testing sets.
4. **Model Training** — Trains a **Support Vector Classifier (SVC)** on the training data.
5. **Model Persistence** — Saves the trained model using `pickle` for reuse without retraining.
6. **Evaluation** — Loads the saved model and evaluates it on the testing set, achieving **80% accuracy**.
7. **Prediction** — Takes user-provided medical data as input and predicts diabetes risk using the trained model.
   
## Tech Stack

| | |
|---|---|
| **Language** | Python 3.13.5 |
| **IDE** | Google Colab Notebook |
| **Libraries** | NumPy 2.1.3, Pandas 2.2.3, scikit-learn 1.6.1, Pickle, PrettyTable 3.16.0, Astropy 7.0.0 |
| **Algorithm** | Support Vector Classifier (SVC) |
| **Accuracy** | 80% |

## Repository Contents

- `Diabetes_Prediction_System.ipynb` — Full notebook with step-by-step code, explanations, training, and evaluation.
- `diabetes_data.csv` — Sample dataset used for training and testing.
- `link.txt` — Link to the deployed web application.

## Conclusion

The analysis shows that diabetes risk in this dataset is strongly influenced by key medical parameters — particularly Glucose levels, BMI, and Age. Higher values in these features significantly increase the probability of a positive diagnosis. Using the Support Vector Classifier, the model achieved **80% accuracy** on testing data.

Despite the small dataset size (100 instances), the model demonstrates how physiological and demographic factors can be used to assess health risk. Future improvements — such as feature scaling and a larger, more balanced dataset — could further enhance predictive performance.

