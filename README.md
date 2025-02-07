# 📌 Machine Learning Pipeline for Student Performance Prediction

This repository contains a complete **machine learning pipeline** for predicting student performance based on demographic and academic factors. The pipeline includes **data ingestion, preprocessing, model training, and deployment** using Flask.

---

## 🚀 Features
- **Data Ingestion**: Reads student performance data, preprocesses it, and splits it into training and testing sets.
- **Model Training**: Trains and evaluates multiple regression models (Random Forest, XGBoost, CatBoost, etc.).
- **Prediction Pipeline**: Uses the trained model to predict student scores based on input features.
- **Flask Web App**: Provides a simple UI to input student data and get predictions.

---

## 📚 Project Structure
```
Student-performance-prediction/
│-- artifacts/               # Stores generated artifacts (datasets, models, preprocessor)
│-- logs/                    # Stores application logs
│-- notebook/                # Jupyter Notebooks for exploration
│-- src/                     # Source code for ML pipeline
│   ├── components/          # Data processing components
│   │   ├── data_ingestion.py       # Handles reading, preprocessing, and splitting dataset
│   │   ├── model_trainer.py        # Trains multiple regression models
│   │   ├── __init__.py             # Package initialization
│   ├── pipeline/            # Training and prediction pipelines
│   │   ├── predict_pipeline.py     # Loads the trained model and makes predictions
│   │   ├── train_pipeline.py       # Placeholder for training pipeline
│   │   ├── __init__.py             # Package initialization
│   ├── utils.py             # Utility functions (saving/loading models, evaluation)
│   ├── exception.py         # Custom exception handling
│   ├── logger.py            # Logging setup
│-- templates/               # HTML templates for Flask UI
│-- venv/                    # Virtual environment (not included in repo)
│-- app.py                   # Flask application for web interface
│-- requirements.txt         # Dependencies
│-- setup.py                 # Package setup
│-- README.md                # Project documentation (this file)
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/Student-performance-prediction.git
cd Student-performance-prediction
```

### 2️⃣ Create a Virtual Environment (Optional but Recommended)
```sh
conda create --name mlproject python=3.8 -y
conda activate mlproject
```

### 3️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

---

## 🏢 Running the Project

### 1️⃣ Run Data Pipeline and Model Training
```sh
python src/components/data_ingestion.py
```
This will:
- Load the dataset
- Preprocess the data
- Split it into train and test sets
- Train and evaluate the model
- Save the best-performing model as `model.pkl`

---

### 2️⃣ Run the Flask App
```sh
python app.py
```
The app will be available at:  
🔗 **http://127.0.0.1:5000/**

---

## 🏆 Model Performance
- The best-performing model is selected based on **R² score**.
- The evaluation results are logged.

---

## 📊 Technologies Used
- **Python**
- **Scikit-learn** (for ML models)
- **Pandas, NumPy** (for data manipulation)
- **Flask** (for web deployment)
- **CatBoost, XGBoost** (for boosting-based regression)

---

## 📝 Contributing
Feel free to fork this repository and submit pull requests. For major changes, open an issue first.

---

## 📩 Contact
👨‍💻 **Author:** Vishwesh  
📧 Email: vishweshhampali@gmail.com  