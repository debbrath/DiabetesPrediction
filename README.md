# Diabetes Prediction System (FastAPI + Render + Docker)
A production-grade FastAPI web application designed to predict diabetes based on patient health data. It emphasizes machine learning deployment, asynchronous REST API design and modern UI development, delivering predictions through both an interactive dashboard and a RESTful endpoint.

The predictive system is trained using the Pima Indians Diabetes Dataset, applying multiple algorithms such as Logistic Regression, Random Forest to ensure accuracy and performance.

<br/>

## ⚡ Live Deployment 
 📦  Live API:  [Swagger Docs](https://diabetesprediction-2zpf.onrender.com/docs)
 
 📦  Live APPLICATION: [Diabetes Prediction](https://diabetesprediction-2zpf.onrender.com/)

<br/>

## 🔍 Features
- **Trained ML Model:**  Train model on the Pima Indians Diabetes dataset to provide reliable diabetes predictions.
- **FastAPI:** Implements a RESTful API with clear, asynchronous, and well-documented routes.
- **Schema Validation:** Enforces type safety using Pydantic for robust data handling.
- **Interactive API Docs:** Automatically generated documentation via Swagger UI and ReDoc.
- **Docker:** Easily deployable using Docker containers.
- **Deployed on Render:** Hosted live with automatic documentation available out of the box.


<br/>

## ⚙️ Technology Overview
- **Backend:** FastAPI, Uvicorn
- **Frontend:** HTML, CSS, JavaScript
- **Machine Learning:** Scikit-learn using the Pima Indians Diabetes dataset
- **Deployment Tools:** Docker, Docker Compose, and hosted on Render


<br/>

## 📦 Project Structure

```
DiabetesPrediction/
│
├── app/
│   ├── __pycache__/              # Auto-generated Python cache
│   ├── __init__.py               # Makes the app a package
│   ├── main.py                   # FastAPI entry point or app logic
│   ├── schemas.py                # Pydantic models (input/output validation)
│   ├── metrics.json              # Model performance metrics
│   ├── diabetes_model.pkl        # Trained machine learning model
│   └── static/                   # Static front-end files
│       ├── index.html
│       ├── script.js
│       └── style.css
│
├── data/
│   └── diabetes.csv              # Dataset used for training
│
├── model/
│   └── train_model.py            # Model training script
│
├── Dockerfile                    # Docker container instructions
├── docker-compose.yml           # Docker Compose for service management
├── metrics.json                  # (Duplicate or root-level copy)
├── README.md                     # Project documentation
└── requirements.txt             # Python dependencies

```
<br/>

## 🛠 Installation & Local Development
### 1. Prerequisites
```bash
- Python 3.13.7
- pip (Python package manager)
```
### 2. Clone the repository
```bash
git clone https://github.com/debbrath/DiabetesPrediction.git
cd DiabetesPrediction
```
### 3. Install dependencies
```bash
pip install -r requirements.txt
```
### 4. Train the model (if not already trained)
```bash
# For training model and build joblib
python train_model.py
```
### 5. Run the API locally
```bash
uvicorn app.main:app --reload
```
<br/>
  
## 🚪 API 

| Method | Endpoint     | Description                                                  |
|--------|--------------|--------------------------------------------------------------|
| GET    | /health      | Check if the API is up and running                           |
| GET    | /info        | Get details about the trained machine learning model         |
| GET    | /metrics     | Retrieve best-performing algorithm and its AUC score         |
| POST   | /predict     | Submit patient data to receive a diabetes prediction         |


```

📸 Screenshots
```
![Screenshot](https://github.com/debbrath/DiabetesPrediction/blob/main/image/2025-08-19%2018_11_52-Settings.png)

✍️ Author

Debbrath Debnath

📫 [Connect on LinkedIn](https://www.linkedin.com/in/debbrathdebnath/)

🌐 [GitHub Profile](https://github.com/debbrath)
