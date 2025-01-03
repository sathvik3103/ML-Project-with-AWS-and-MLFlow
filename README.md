# Wine Quality Prediction with AWS and MLFlow

## Overview
This project implements a machine learning model to predict wine quality using the ElasticNet algorithm. It demonstrates MLflow integration for experiment tracking, model versioning, and deployment.

## Project Structure
```
wine-quality-prediction/
│
├── app.py            # Main training script
├── requirements.txt    # Project dependencies
└── README.md          # Project documentation
```

## Features
* Wine quality prediction using ElasticNet regression
* MLflow experiment tracking and model logging
* Remote model registry integration
* Model performance metrics (RMSE, MAE, R2)
* Cross-validation and hyperparameter tuning

## Requirements
To run this project, you need the following dependencies:
```
pandas
numpy
scikit-learn
mlflow
```

You can install all requirements using:
```
pip install -r requirements.txt
```

## Dataset
The project uses the Wine Quality dataset from the UCI Machine Learning Repository. The dataset contains various chemical properties of wines and their quality ratings.


## MLflow Tracking
The project is configured to use a remote MLflow tracking server. To view the experiments:
1. Access the MLflow UI at: `http://ec2-52-207-245-90.compute-1.amazonaws.com:5000/` (now deleted)
2. View experiments, metrics, and model versions

## Model Features
The model uses the following features to predict wine quality:
* Fixed acidity
* Volatile acidity
* Citric acid
* Residual sugar
* Chlorides
* Free sulfur dioxide
* Total sulfur dioxide
* Density
* pH
* Sulphates
* Alcohol

## Performance Metrics
The model's performance is evaluated using:
* Root Mean Square Error (RMSE)
* Mean Absolute Error (MAE)
* R-squared (R2) score

## Model Registry
The trained model is automatically registered in MLflow's Model Registry as "ElasticnetWineModel" when using a remote tracking server.

## Proof of Deployment:

## Output in CLI:
![Output in CLI](https://github.com/user-attachments/assets/f323cc63-b52a-4dc5-9436-a30af1852c79)


## MLFlow UI hosted on AWS EC2 instance:

![MLflow UI hosted in EC2 instance](https://github.com/user-attachments/assets/d60264f7-13b1-4700-9a5f-83d3b4559dde)


## ML Model stored in AWS S3 bucket:
![ML model stored in S3 bucket](https://github.com/user-attachments/assets/9098f6dd-b13c-40d5-8974-15b91790a8f4)






