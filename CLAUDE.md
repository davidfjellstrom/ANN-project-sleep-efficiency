# Project Instructions – Sleep Efficiency ANN

## About this project
This is a group school project for a YrkesHögskola (vocational college) course on
Artificial Neural Networks (ANN). The project is built by two students who are
not experts in the field — keep that in mind when suggesting solutions.

## Our goal
We are predicting **sleep efficiency** (a value between 0 and 1) using lifestyle
factors such as caffeine intake, alcohol consumption, exercise frequency, smoking
habits, age, and sleep duration.

This is a **regression problem** solved with an ANN model built in Keras / TensorFlow.

## Dataset
- File: `Sleep_Efficiency.csv`
- Source: Kaggle – Sleep Efficiency Dataset
- 452 rows, 15 columns
- Target variable: `Sleep efficiency` (float, 0–1)
- Some missing values in: Awakenings, Caffeine consumption, Alcohol consumption, Exercise frequency

## Assignment requirements
1. Perform EDA – describe the data and relationships between variables
2. Build a simple ANN model
3. Evaluate the model
4. Present results as a data story (~15 min presentation)
5. Explain why the model is valuable for a business

## Code guidelines
- Language: **Python**, using Jupyter Notebook (.ipynb)
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, tensorflow/keras
- Code should be **well structured** and clearly divided into sections
- Comments should be natural and not over-engineered
- The overall language level should match two vocational college students –
  avoid overly academic or AI-sounding explanations

## Tone and language
- Code and comments are written in **English**
- Any markdown text cells in the notebook can be in English
- Keep explanations simple and clear — we understand the concepts but are not experts

## Project structure
```
ANN_PROJECT_SLEEP_EFFICIENCY/
├── CLAUDE.md                        ← this file
├── Sleep_Efficiency.csv             ← the dataset
└── sleep_efficiency_project.ipynb   ← the main notebook
```

## What we have done so far
- Chose the dataset (Sleep Efficiency from Kaggle)
- Created a base notebook with the following sections:
  1. Import Libraries
  2. Load Dataset
  3. Data Cleaning (missing values, encoding, dropping unused columns)
  4. EDA (histograms, boxplots, scatterplots, correlation matrix)
  5. Prepare Data (train/test split, StandardScaler)
  6. Build ANN Model (Sequential, two hidden layers: 64 → 32 → 1)
  7. Train Model (100 epochs, batch_size=16, validation_split=0.2)
  8. Evaluate Model (MSE, RMSE, MAE, R², actual vs predicted plot)
  9. Save Model and Scaler
  10. Summary and Conclusions

## Business angle for the presentation
A health app or insurance company could use this model to give personalized
sleep recommendations based on a user's lifestyle. By adjusting factors like
caffeine intake or exercise frequency, the model can show how sleep efficiency
would change — helping users make better decisions for their health.
