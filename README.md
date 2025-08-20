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

python -m pip install -r requirements.txt
python train_model.py

📦 Project Structure

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
![Screenshot](https://github.com/debbrath/DiabetesPrediction/blob/main/image/2025-08-19%2018_11_52-Settings.png)

✍️ Author

Debbrath Debnath

📫 [Connect on LinkedIn](https://www.linkedin.com/in/debbrathdebnath/)

🌐 [GitHub Profile](https://github.com/debbrath)
