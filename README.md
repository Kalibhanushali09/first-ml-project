End-to-End Machine Learning Project

This repository contains an end-to-end Machine Learning project that covers the complete ML lifecycle — from data ingestion and preprocessing to model training, evaluation, and deployment readiness.

Project Overview

This project is designed to demonstrate how a production-ready machine learning pipeline is built using industry best practices such as:

Modular code structure

Reusable components

Proper packaging with setup.py

Model serialization

Web framework integration (Flask)

Tech Stack & Libraries Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

CatBoost

XGBoost

Flask

Dill (for model serialization)

📂 Project Structure
first_ml_project/
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── train_pipeline.py
│   │   └── predict_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── artifacts/
│   ├── train.csv
│   ├── test.csv
│   └── model.pkl
│
├── app.py
├── requirements.txt
├── setup.py
├── README.md
└── .gitignore

Installation & Setup
1️⃣ Clone the repository
git clone <repository-url>
cd first_ml_project

2️⃣ Create a virtual environment
python -m venv venv


Activate it:

Windows

venv\Scripts\activate


Mac/Linux

source venv/bin/activate

3️⃣ Install dependencies
pip install -r requirements.txt


Or install the project as a package:

pip install -e .

▶️ How to Run the Project
Train the model
python src/pipeline/train_pipeline.py

Run the Flask app
python app.py

ML Pipeline Flow

Data Ingestion

Loads raw data

Splits data into train and test sets

Data Transformation

Handles missing values

Feature scaling and encoding

Model Training

Trains multiple ML models

Compares performance

Saves the best model

Prediction Pipeline

Loads trained model

Makes predictions on new data

Model Saving

Models are serialized using Dill

Stored inside the artifacts/ directory

Easily reusable for inference and deployment

Deployment Ready

The project includes Flask, making it easy to:

Build APIs

Serve ML models

Integrate with frontend applications