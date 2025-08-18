# Diabetes Prediction (FastAPI + Docker)

# 🌍 Live Render Deployment 
# 📦  Live API:  [Swagger Docs](https://diabetesprediction-2zpf.onrender.com/docs)
# 📦  Live APPLICATION: [Heart Disease Prediction](https://diabetesprediction-2zpf.onrender.com/)


🫀 Diabetes Prediction API

A FastAPI-powered REST API that serves predictions from a machine learning model trained to detect diabetes. This project focuses on containerization with Docker and deployment to the cloud using Render. Built as part of a hands-on assignment to demonstrate practical DevOps, ML, and API development skills.

🔍 Features

✅ /health — Health check endpoint

🔮 /predict — Accepts patient data and returns diabetes prediction (True/False)

📄 /metrics — Return classification metrics

🐳 Dockerized for local and cloud deployment

☁️ Live deployment on Render


🧠 Model

Trained on the Diabetes dataset

Model type: LogisticRegression,RandomForest

Saved using joblib and served as a REST API

🚀 Tech Stack

FastAPI

scikit-learn

Docker & Docker Compose

Render (for cloud deployment)

Pydantic (for input validation)

📦 Installation (Local)
bash
Copy
Edit
git clone https://github.com/debbrath/DiabetesPrediction.git
cd DiabetesPrediction
docker-compose up --build
Then visit: http://localhost:8000/docs

📦 Train model locally
```bash
python -m pip install -r requirements.txt
python train_model.py
# This will create model/heart_model.joblib

📁 Project Structure

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



📸 Screenshots
```
![Screenshot](https://github.com/debbrath/FastAPI_Docker_HeartDiseasePrediction/blob/main/Image/2025-08-12%2013_54_19-Window.png)

![Screenshot](https://github.com/debbrath/FastAPI_Docker_HeartDiseasePrediction/blob/main/Image/2025-08-12%2013_57_32-Window.png)

![Screenshot](https://github.com/debbrath/FastAPI_Docker_HeartDiseasePrediction/blob/main/Image/2025-08-12%2016_55_08-Window.png)

![Screenshot](https://github.com/debbrath/FastAPI_Docker_HeartDiseasePrediction/blob/main/Image/2025-08-14%2011_59_10-Window.png)




✍️ Author

Debbrath Debnath

📫 [Connect on LinkedIn](https://www.linkedin.com/in/debbrathdebnath/)

🌐 [GitHub Profile](https://github.com/debbrath)
