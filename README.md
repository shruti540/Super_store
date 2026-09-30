🛒 Super Store Sales Prediction

📌 Project Overview

Super Store Sales Prediction is a Machine Learning project that predicts the sales of an item at a particular outlet based on different item and outlet-related features.

The project uses K-Nearest Neighbors (KNN) Regression to predict "Item_Outlet_Sales". The dataset is preprocessed and normalized before training the Machine Learning model.

A Flask web application is also developed to allow users to enter item and outlet information and receive a predicted sales value.

---

🎯 Objectives

- Predict item sales for different outlets.
- Analyze item and outlet-related features.
- Perform data preprocessing and normalization.
- Train a KNN Regression model.
- Tune the KNN model parameters.
- Save the trained model using Pickle.
- Create a web application for sales prediction.

---

🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- KNN Regression
- Flask
- HTML/CSS
- Jupyter Notebook
- Pickle

---

📊 Dataset

The project uses an outlet sales dataset where the target variable is:

Item_Outlet_Sales

The model uses item and outlet features such as:

- Item Weight
- Item Fat Content
- Item Visibility
- Item MRP
- Item Type
- Outlet Identifier
- Outlet Size
- Outlet Location Type
- Outlet Establishment Year
- Outlet Type

---

🔄 Project Workflow

Dataset
   ↓
Data Preprocessing
   ↓
Feature Selection
   ↓
Data Normalization
   ↓
Train-Test Split
   ↓
KNN Regression
   ↓
Hyperparameter Tuning
   ↓
Model Evaluation
   ↓
Save Model
   ↓
Flask Web Application
   ↓
Sales Prediction

---

🤖 Machine Learning Algorithm

K-Nearest Neighbors Regression

The project uses KNN Regression for predicting continuous sales values.

The KNN model finds the nearest data points to a given input and uses them to estimate the output value.

The project also uses:

- "GridSearchCV"
- "RandomizedSearchCV"

for finding suitable KNN parameters.

The final model is saved using Pickle for use in the Flask application.

---

📈 Model Evaluation

The model performance is evaluated using the R² Score.

accuracy = r2_score(y_test, y_pred)

The R² score is used to measure how well the model explains the variation in the target sales values.

---

🌐 Flask Web Application

The Flask application loads the trained KNN model and provides a prediction interface.

The application accepts information such as:

- Item Weight
- Item Fat Content
- Item Visibility
- Item MRP
- Item Type
- Outlet Identifier
- Outlet Size
- Outlet Location Type
- Outlet Establishment Year
- Outlet Type

The entered information is converted into the same feature structure used during model training before making the prediction.

---

📂 Project Structure

Super-Store-Sales-Prediction/
│
├── app.py
├── KNN Regression.ipynb
├── dataset.csv
├── knn_regression_model.pkl
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
│
├── requirements.txt
└── README.md

---

🚀 How to Run the Project

1. Clone the Repository

git clone YOUR_GITHUB_REPOSITORY_LINK

2. Open the Project Folder

cd Super-Store-Sales-Prediction

3. Install Required Libraries

pip install pandas numpy scikit-learn flask

Or use:

pip install -r requirements.txt

4. Run the Flask Application

python app.py

The application will run locally and can be opened in a web browser.

---

💻 Prediction Process

The Flask application:

1. Takes input from the user.
2. Converts the input into numerical features.
3. Creates the required feature DataFrame.
4. Creates dummy variables for categorical features.
5. Arranges the columns in the training order.
6. Loads the trained KNN model.
7. Generates the predicted outlet sales.
8. Displays the prediction on the web page.

The application specifically reindexes the input using the model's training columns so that the prediction receives features in the expected order.

---

🌟 Key Features

- Machine Learning-based sales prediction
- KNN Regression
- Data normalization
- Hyperparameter tuning
- R² model evaluation
- Pickle model saving/loading
- Flask-based web interface
- Categorical feature encoding
- Real-time prediction through user input

---

🔮 Future Scope

- Use larger and more recent sales datasets.
- Compare KNN with Random Forest, XGBoost, and other regression algorithms.
- Improve model accuracy through feature engineering.
- Add graphical sales analysis.
- Deploy the Flask application online.
- Add historical sales visualization.
- Add a dashboard for outlet-wise and item-wise analysis.
📜 License

This project is created for educational and learning purposes.
