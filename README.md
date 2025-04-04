🏠 House Price Prediction – California Housing Dataset
📌 Project Overview
This project involves building a regression model to predict housing prices in California using the California Housing Dataset from scikit-learn. The model is trained using XGBoost, a powerful and efficient implementation of gradient boosting.
🧠 Objective
To develop a machine learning model that accurately predicts median house prices based on features such as:
Median income
House age
Average rooms per household
Location-based features (latitude, longitude)
And more...
📦 Technologies Used
Python
NumPy & Pandas (Data manipulation)
Matplotlib & Seaborn (Visualization)
Scikit-learn (Dataset & Preprocessing)
XGBoost (Model training)
Jupyter Notebook / Python Scripts
📊 Dataset Information
Source: Scikit-learn’s built-in fetch_california_housing()
Target Variable: MedHouseVal (Median house value for California districts)
Number of Samples: 20,640
Number of Features: 8 numeric features
Data Type: Numeric, Continuous
⚙️ Workflow
Import Libraries & Load Data
Used fetch_california_housing() to load the dataset.
Exploratory Data Analysis (EDA)
Visualized distributions and correlations using Seaborn and Matplotlib.
Data Preprocessing
Checked for missing values
Performed train-test split (80/20)
Model Selection
Chose XGBRegressor for its efficiency and performance on structured/tabular data.
Model Training
Trained the XGBoost model on the training dataset.
Model Evaluation
Evaluated using metrics like R² score and Mean Absolute Error.
📈 Evaluation Metrics
R² Score: Measures how well predictions approximate the actual data.
MAE (Mean Absolute Error): Measures the average magnitude of the errors.
r2_score = metrics.r2_score(y_test, predictions)
mae = metrics.mean_absolute_error(y_test, predictions)
💾 Model Saving
You can save the trained model using:
import joblib
joblib.dump(model, 'housing.sav')
🚀 Future Work
Hyperparameter tuning using GridSearchCV or RandomizedSearchCV
Feature engineering
Deploy model using Flask/Django or on cloud platforms (AWS, GCP, Heroku)
📁 Project Structure
├── data/                 # Raw or processed data (optional)
├── notebook.ipynb        # Jupyter notebook with full analysis
├── housing.sav           # Saved trained model
├── README.md             # Project documentation
👤 Author
Rahul Pandey
📧 rahulpandey02124@email.com
