# 🌊 Rising Waters: A Machine Learning Approach to Flood Prediction

A Machine Learning-based web application that predicts flood risk using historical weather data such as **temperature, humidity, cloud cover, and seasonal rainfall**. The application is built using **Python**, **Flask**, and **Scikit-learn**, providing users with an easy-to-use interface for flood prediction.

---

## 🚀 Features

- Predicts flood risk using Machine Learning.
- Interactive web interface built with Flask.
- Compares multiple ML algorithms and selects the best-performing model.
- Stores prediction history using SQLite.
- Supports retraining with updated datasets.
- Clean and responsive UI.

---

## 🏗️ Architecture

```
Browser
   │
   ▼
Presentation Layer (HTML/CSS)
   │
   ▼
Flask Application
   │
   ▼
Machine Learning Layer
(model.pkl & scaler.pkl)
   │
   ▼
Data Layer
```

---

## 📂 Project Structure

```
flood_prediction_project/
│
├── app.py
├── train_model.py
├── requirements.txt
│
├── data/
│   └── flood_dataset.xlsx
│
├── model/
│   ├── model.pkl
│   ├── scaler.pkl
│   └── metadata.json
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── form.html
│   ├── result.html
│   └── history.html
│
├── static/
│   └── css/
│       └── style.css
│
└── history.db
```

---

## 🛠️ Technologies Used

- Python
- Flask
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- SQLite
- HTML5
- CSS3
- JavaScript

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/mangasuvarna/flood_prediction_project.git
cd flood_prediction_project
```

### Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install required packages

```bash
pip install -r requirements.txt
```

---

## 🧠 Train the Model

Run the following command:

```bash
python train_model.py
```

The script will:

- Load the dataset
- Train four Machine Learning models
- Compare their performance
- Save the best-performing model as:

```
model/model.pkl
model/scaler.pkl
model/metadata.json
```

---

## ▶️ Run the Application

```bash
python app.py
```

Open your browser and visit:

```
http://127.0.0.1:5000
```

---

## 📄 Application Pages

### 🏠 Home

Displays the project dashboard and active model information.

### 🌧️ New Prediction

Enter weather parameters to predict flood risk.

### 📊 Prediction History

Displays all previous predictions stored in a local SQLite database.

---

## 🤖 Machine Learning Models Used

- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- XGBoost

The application automatically selects the best-performing model based on evaluation metrics.

---

## 📊 Dataset

The model is trained using historical weather data containing:

- Temperature
- Humidity
- Cloud Cover
- Seasonal Rainfall

Target Variable:

- Flood
- No Flood

---

## 🔄 Retraining

Whenever the dataset is updated, simply run:

```bash
python train_model.py
```

The application will retrain all models and automatically save the best one.

---

## 🚀 Deployment

For production deployment, install Gunicorn:

```bash
pip install gunicorn
```

Run the application using:

```bash
gunicorn -w 2 -b 0.0.0.0:8080 app:app
```

This project can be deployed on platforms such as:

- Render
- Railway
- IBM Cloud
- AWS
- Azure
- Google Cloud

---

## 📸 Screenshots

You can add screenshots of:

- Home Page
- Prediction Form
- Prediction Result
- History Page

---

## 🔮 Future Enhancements

- Live Weather API Integration
- Interactive Flood Risk Maps
- SMS & Email Alerts
- User Authentication
- Cloud Database Support
- Real-Time Weather Forecast Integration

---

## 👩‍💻 Author

**Suvarna M**

GitHub: https://github.com/mangasuvarna

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
