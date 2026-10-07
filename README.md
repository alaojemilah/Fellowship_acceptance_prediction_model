# Fellowship Acceptance Prediction Model

## Problem Statement
The goal of this project is to predict whether a person will be accepted into a fellowship or not based on their personal information.

This is a *classification problem* and the output belongs to one of two categories:
- *1* = Accepted
- *0* = Not Accepted

## Dataset
- *Source:* fellowship_dataset (custom dataset)
- *Total entries:* 100
- *Features:*
  - Gender (Female = 1, Male = 0)
  - Age
  - City (encoded 0-10)
  - Graduate (Yes = 1, No = 0)
- *Target:* Accepted (1 or 0)

## What I Did
- Preprocessed the dataset and handled categorical encoding
  - Gender: Female = 1, Male = 0
  - Graduate: Yes = 1, No = 0
  - City: encoded 0-10
- Split data into training and test sets (80/20 split, random_state=42)
- Used stratified splitting to maintain class balance
- Scaled features using feature scaling
- Trained multiple machine learning models
- Created a prediction function to test on unseen data

## Models Tested & Results

| Model | Parameters | Accuracy |
|---|---|---|
| Logistic Regression | max_iter=800 | *100%* |
| Decision Tree | max_depth=2, random_state=42 | *100%* |
| Support Vector Classifier | kernel=rbf, C=0.5, gamma=scale | *100%* |

## Best Model
All three models achieved *100% accuracy*. However this is likely due to the small dataset size of only 100 entries. A larger and more diverse dataset would give a more realistic evaluation of model performance.

## Key Takeaways
- All models achieved 100% accuracy on this dataset
- The high accuracy is likely influenced by the small dataset size (100 entries)
- Stratified splitting ensured balanced class representation in training and test sets
- A larger dataset would be needed to validate real-world performance
- This project demonstrates the importance of dataset size in evaluating model reliability

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn

## Author
Jemilah Alao | Data Analyst
[LinkedIn](https://www.linkedin.com/in/jemilah-alao-8a684528a)
