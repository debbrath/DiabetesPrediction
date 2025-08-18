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
diabetesprediction/
│
├── model/
│   ├── train_model.py
│   ├── diabetes_model.pkl
│   └── metrics.json
│
├── backend/
│   ├── main.py
│   ├── schemas.py
│   ├── diabetes_model.pkl
│   ├── metrics.json
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── .gitignore
└── README.md

```

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
