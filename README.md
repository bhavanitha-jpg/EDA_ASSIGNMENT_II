# Student Performance EDA and Deep Learning

## 1. Project Overview

This project explores student Mathematics performance using Exploratory Data Analysis (EDA), data visualization, statistical analysis, and a deep learning model.

The project uses the Student Performance dataset from the UCI Machine Learning Repository. It analyzes student demographics, family background, study habits, absences, and academic performance.

## 2. Objectives

- Explore the dataset and identify patterns in student performance.
- Clean and preprocess the data.
- Visualize grade distributions and relationships between features.
- Develop a neural network to predict pass/fail outcomes.
- Evaluate the model using classification metrics and visualizations.

## 3. Dataset

**Source:** UCI Machine Learning Repository — Student Performance

https://archive.ics.uci.edu/dataset/320/student+performance

The Mathematics dataset contains 395 student records and 33 attributes.

The target is defined as:
- Pass (1): final grade G3 >= 10
- Fail (0): final grade G3 < 10

The final grade and earlier period grades are excluded from the model inputs to prevent grade leakage.

## 4. Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- TensorFlow / Keras
- Visual Studio Code and Jupyter Notebook

## 5. Exploratory Data Analysis

The project includes:
- Final grade distribution histogram
- Study time versus final grade boxplot
- Correlation heatmap
- Past failures versus final grade boxplot
- Study time distribution chart

## 6. Deep Learning

A Multilayer Perceptron (MLP) is trained using processed numerical and categorical features. The model uses ReLU hidden layers, dropout, and a sigmoid output layer.

The data is divided into training, validation, and testing sets.

## 7. Evaluation

Model performance is assessed using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrix
- Training and validation accuracy/loss plots

Actual results are saved in `outputs/model_evaluation_results.csv`.

## 8. Project Structure

```text
Student_Performance_EDA/
├── data/
│   └── student-mat.csv
├── notebooks/
│   └── Student_Performance_EDA.ipynb
├── outputs/
│   ├── figures/
│   ├── model_evaluation_results.csv
│   └── student_performance_model.keras
├── requirements.txt
└── README.md
```

## 9. How to Run

1. Clone or download the repository.
2. Create and activate a Python virtual environment.
3. Install dependencies using `pip install -r requirements.txt`.
4. Place `student-mat.csv` in the `data` folder.
5. Open the notebook and run its cells in order.

## 10. Limitations and Future Scope

The dataset is relatively small and represents students from two Portuguese schools. The model's results may not generalize to other schools or countries. Future work could evaluate other machine learning models, use additional datasets, and investigate explainable AI techniques.

