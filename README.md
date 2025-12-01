# Daily Workout Predictor Using Machine Learning

This project uses machine learning to recommend a suitable workout for the day based on self-collected lifestyle data. The goal is to help users decide between strength training, cardio, or rest by using daily information such as sleep, stress, soreness, energy level, available time, previous workouts, and health conditions.

# Dataset

The dataset was recorded manually over several weeks. Each row represents one day and includes features such as:

- Sleep hours  
- Bedtime and wake time  
- Soreness, stress, energy, motivation  
- Sickness level  
- Time available for workout  
- Previous day strength or cardio  
- Whether the previous day was a rest day  
- Whether it is a workday  
- Injury indicator  
- Recommended workout label (strength, cardio, rest)


File included:
workout_data.csv

# Model Overview

Multiple models were tested, including:

- Random Forest
- Logistic Regression
- K-Nearest Neighbors

Random Forest achieved the best overall performance on this small dataset.
Simple linear models struggled due to limited data and overlapping feature patterns.

A few safety rules were added to improve real-world use, such as automatically recommending rest when sick, injured, or when available workout time is too low.

# Notebook

The full training process, evaluation, and prediction examples are in:
Lei_Code.ipynb

The notebook shows:

- Data preprocessing
- Model training
- Evaluation results
- Confusion matrices
- Example daily predictions using the trained model

# How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Zlei1997/Daily-Workout-Predictor-Using-Machine-Learning.git


# License

This project is released under the MIT License.
