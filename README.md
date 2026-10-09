# 🚗 Car Price Prediction Using Machine Learning & MLflow

## 📌 Project Overview

This project predicts car prices using machine learning techniques. A **Random Forest Regressor** is used to build the prediction model, and **GridSearchCV** is used for hyperparameter tuning to find the best model configuration.

**MLflow** is integrated to track experiments, log hyperparameters and evaluation metrics, and save trained model artifacts for reproducibility and model management.

## 🎯 Project Objectives

* Build a machine learning model to predict car prices.
* Perform data preprocessing and categorical encoding.
* Optimize model performance using GridSearchCV.
* Evaluate the model using regression metrics.
* Track experiments and manage model artifacts using MLflow.

## 🛠️ Technologies Used

* **Python** – Programming language
* **Pandas & NumPy** – Data manipulation and numerical operations
* **Scikit-learn** – Model training, hyperparameter tuning, and evaluation
* **MLflow** – Experiment tracking and model logging
* **Jupyter Notebook** – Development and experimentation

## ⚙️ Machine Learning Workflow

1. **Data Collection:** Load the car price dataset.
2. **Data Preprocessing:** Clean the data and encode categorical variables.
3. **Feature and Target Separation:** Separate input features and the target price.
4. **Train-Test Split:** Divide the dataset into training and testing sets.
5. **Model Training:** Train a Random Forest Regressor.
6. **Hyperparameter Tuning:** Use GridSearchCV with cross-validation to identify the best hyperparameters.
7. **Model Evaluation:** Evaluate predictions using R² score, Mean Absolute Error (MAE), and Mean Squared Error (MSE).
8. **Experiment Tracking:** Log parameters, metrics, and model artifacts using MLflow.

## 📊 Model Evaluation Metrics

The model is evaluated using the following metrics:

* **R² Score:** Measures how well the model explains the variation in car prices. Higher values generally indicate better performance.
* **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices.
* **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted prices.

The actual model performance depends on the dataset, features, and selected hyperparameters.

## 📈 MLflow Experiment Tracking

MLflow is used to organize and track machine learning experiments.

The project logs:

* Best hyperparameters selected by GridSearchCV.
* Model evaluation metrics, including MSE, MAE, and R² score.
* The trained Random Forest model as an artifact.
* The registered model name, when model registration is configured.

**Experiment name:** `Car_Price_Prediction_Experiment`

**Registered model name:** `best_carpridiction_model`

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

Replace the placeholders with your actual GitHub repository URL and folder name.

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate the environment.

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install pandas numpy scikit-learn mlflow jupyter
```

If you use a `requirements.txt` file, you can instead install the dependencies with:

```bash
pip install -r requirements.txt
```

### 4. Start the MLflow tracking server

```bash
mlflow server --host 127.0.0.1 --port 5000
```

Keep the server running in a terminal.

### 5. Run the project

Open your Jupyter Notebook and execute the cells in order, from data preprocessing through model training and evaluation.

The tracking URI used in the project is:

```python
mlflow.set_tracking_uri("http://localhost:5000")
```

### 6. View experiment results

Open the following address in your browser:

http://localhost:5000

You can explore experiment runs, compare logged metrics, inspect hyperparameters, and view model artifacts.

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── data/
│   └── car_data.csv
│
├── notebooks/
│   └── car_price_prediction.ipynb
│
├── mlruns/                 # Local MLflow artifacts, if applicable
├── requirements.txt
├── README.md
└── .gitignore
```

*Note: Adjust the folder structure and filenames to match your actual repository. MLflow artifacts may be stored in a separate location depending on your tracking server configuration.*

## 🔮 Future Improvements

* Compare Random Forest with other regression algorithms.
* Improve model performance through feature engineering.
* Add visualizations for actual versus predicted prices.
* Build an interactive web application for price predictions.
* Deploy the trained model using a suitable deployment platform.
* Integrate automated testing and model monitoring.

## 👨‍💻 Author

**Your Name**

GitHub: (https://github.com/akshay-np973)

## 📄 License

This project is intended for educational and machine learning practice. Add a suitable open-source license if you wish to allow others to reuse or modify the code.
