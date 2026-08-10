# 🍔 Food Delivery Time Prediction

A Machine Learning-based web application that predicts the estimated food delivery time based on various delivery-related factors.

The trained Machine Learning model is integrated with a Flask web application, allowing users to enter delivery details and receive an estimated delivery time through an interactive web interface.

---

## 📌 Project Overview

Food delivery time can depend on several factors such as distance, traffic conditions, preparation time, vehicle type, and other delivery-related information.

This project uses Machine Learning to analyze these factors and predict the estimated delivery time.

The project consists of two main components:

- **Machine Learning Model** – Used to process delivery-related data and predict delivery time.
- **Flask Web Application** – Provides an interactive interface for users to enter information and view the prediction.

---

## ✨ Features

- Interactive Home Page
- About Us Page
- Food Delivery Time Prediction
- Traffic Level consideration
-  Distance consideration
- Preparation Time consideration
- Vehicle Type consideration
- Machine Learning-based prediction
- Flask web application
- Interactive and animated user interface
- Displays estimated delivery time

---

## Technologies Used

### Programming Language

- Python

### Machine Learning

- Pandas
- NumPy
- Scikit-learn
- Joblib

### Web Development

- Flask
- HTML
- CSS
- JavaScript

---

## 📂 Project Structure

```text
Food-Delivery-Time-Prediction/
│
├── static/
│   ├── css/
│   ├── img/
│   ├── js/
│   ├── lib/
│   └── scss/
│
├── templates/
│   ├── about.html
│   ├── base.html
│   ├── index.html
│   └── predict.html
│
├── demo/
│   ├── home.mp4
│   ├── about.mp4
│   └── predict.mp4
│
├── app.py
├── delivery_time_model.pkl
├── delivery_scaler.pkl
├── model_columns.pkl
├── traffic_encoder.pkl
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Project Workflow

```text
User Input
     ↓
Data Preprocessing
     ↓
Feature Encoding
     ↓
Feature Scaling
     ↓
Trained Machine Learning Model
     ↓
Delivery Time Prediction
     ↓
Display Result
```

---

## Machine Learning Implementation

The Machine Learning component is used to predict the estimated food delivery time.

The implementation follows these steps:

### 1. Data Preparation

The delivery dataset is prepared by selecting the required input features and target variable.

### 2. Data Preprocessing

The data is cleaned and prepared before being used for Machine Learning.

### 3. Feature Encoding

Categorical features are converted into numerical representations so that they can be processed by the Machine Learning model.

### 4. Feature Scaling

Numerical features are scaled using the trained scaler.

The same scaler is reused during prediction to ensure that new user inputs are processed consistently with the training data.

### 5. Model Training

The processed dataset is used to train a Machine Learning model for predicting food delivery time.

### 6. Model Saving

The trained model and preprocessing objects are saved using Joblib.

The project contains:

| File | Purpose |
|------|---------|
| `delivery_time_model.pkl` | Trained Machine Learning model |
| `delivery_scaler.pkl` | Feature scaling object |
| `traffic_encoder.pkl` | Traffic feature encoder |
| `model_columns.pkl` | Required model feature columns |

### 7. Prediction

When the user enters delivery information through the Flask application:

1. User input is collected.
2. Input data is preprocessed.
3. Categorical features are encoded.
4. Numerical features are scaled.
5. Processed data is passed to the trained model.
6. Estimated delivery time is generated.
7. The result is displayed on the web page.

---

## Flask Application

The Flask application connects the Machine Learning model with the web interface.

The main application file is:

```text
app.py
```

The Flask application:

- Loads the trained Machine Learning model.
- Loads the required preprocessing objects.
- Accepts user input from the prediction page.
- Processes the input.
- Sends the processed data to the model.
- Displays the predicted delivery time.

---

## Input Features

The prediction system uses delivery-related information such as:

- Distance
- Preparation Time
- Traffic Level
- Vehicle Type
- Other relevant delivery features

---

## Output

The application predicts and displays:

**Estimated Food Delivery Time**

based on the information provided by the user.

---

## Application Demo

The following screen recordings demonstrate the main pages of the application.

### Home Page

[▶️ Watch Home Page Demo](demo/home.mp4)

The Home Page introduces the Food Delivery Time Prediction application and provides navigation to different sections.

### ℹ️ About Us

[▶️ Watch About Us Demo](demo/about.mp4)

The About Us page provides information about the project and its purpose.

### Prediction Page

[▶️ Watch Prediction Page Demo](demo/predict.mp4)

The Prediction Page allows users to enter delivery-related information and obtain an estimated delivery time.

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/DhanyashreePS/Food-Delivery-Time-Prediction.git
```

### 2. Navigate to the Project Folder

```bash
cd Food-Delivery-Time-Prediction
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

For Windows:

```bash
venv\Scripts\activate
```

### 5. Install Required Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Flask Application

```bash
python app.py
```

### 7. Open the Application

Open your browser and visit:

```text
http://127.0.0.1:5000
```

---

## Model Files

The trained Machine Learning model and preprocessing components are included in the repository.

- `delivery_time_model.pkl`
- `delivery_scaler.pkl`
- `traffic_encoder.pkl`
- `model_columns.pkl`

These files allow the Flask application to load the trained model and perform predictions without retraining every time the application starts.

---

## Future Enhancements

- Improve prediction accuracy using larger datasets
- Experiment with different Machine Learning algorithms
- Add real-time distance calculation
- Integrate map and location services
- Add real-time delivery tracking
- Deploy the application online
- Improve prediction visualization
- Add user authentication and order history

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Data preprocessing
- Feature encoding
- Feature scaling
- Machine Learning model training
- Model serialization using Joblib
- Flask application development
- Integrating Machine Learning with a web application
- Building an interactive web interface
- Git and GitHub

---

## Author

**Dhanyashree P S**

Computer Science Engineering Student

---

## Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
