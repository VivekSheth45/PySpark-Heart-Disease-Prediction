# Heart Disease Prediction using PySpark

## Overview

This project leverages PySpark and Machine Learning to predict heart disease based on patient health data. It utilizes a distributed Spark environment with a master-worker node setup, enabling efficient big data processing and predictive modeling.

# Features

🏥 Heart Disease Prediction using ML models

🚀 Distributed Computing with PySpark

📊 Data Processing & Feature Engineering

📈 Visualizations (ROC Curve, Correlation Matrix, Box Plots)

🔥 Optimized Spark Session for scalability

## Project Setup

### Prerequisites

Python 3.x
Apache Spark
PySpark
Jupyter Notebook (optional for analysis)

### Installation
1. Clone the repository
  git clone https://github.com/yourusername/heart-disease-prediction.git
  cd heart-disease-prediction
2. Create and activate a virtual environment
   conda create --name pyspark_env python=3.8
   conda activate pyspark_env
3. Install dependencies
   pip install pyspark pandas matplotlib seaborn scikit-learn

## Spark session setup

We configured a master-worker architecture and initialized the Spark Session with optimized resource allocation:
  from pyspark.sql import SparkSession
  spark = SparkSession.builder \
    .appName("Heart Disease Prediction") \
    .master("spark://<master-node-ip>:7077") \
    .config("spark.executor.memory", "2g") \
    .config("spark.driver.memory", "1g") \
    .config("spark.executor.cores", "2") \
    .config("spark.cores.max", "6") \
    .getOrCreate()

## Data Processing & Visualization

1. Data Cleaning & Preprocessing: Handling missing values, encoding categorical features, and scaling numerical data.

2. Exploratory Data Analysis:

   Correlation Matrix: Understanding feature relationships
   Box Plots: Identifying outliers
   Scatter Plots: Investigating variable distributions
   ROC Curve: Evaluating model performance (AUC = 0.93)

## Model training
  Logistic Regression
  Decision Tree Classifier
  Evaluation: Accuracy, Precision, Recall, F1-score

## Results
✅ Achieved AUC Score of 0.93 using Logistic Regression 🔥
✅ Efficiently processed and analyzed large-scale medical data
✅ Improved model interpretability with feature visualizations

## License
This project is open-source under the MIT License.

## Let's Connect! 💡

If you're passionate about Big Data, PySpark, and AI, let's connect and collaborate! 🚀
viveksheth53@gmail.com
