# 🏨 Hotel Reservation Cancellation Prediction

## 🚀 Project Overview
This project predicts whether a hotel booking will be canceled using an MLOps pipeline. It integrates data ingestion, preprocessing, model training, deployment, and a web application for user interaction.

## 📂 Project Structure
```
├── artifacts/            # Model & processed data
├── config/               # Configuration files (YAML, params, paths)
├── custom_jenkins/       # CI/CD pipeline (Jenkins)
├── notebook/             # Experimentation & EDA
├── pipeline/             # Training pipeline
├── src/                  # Core scripts (data ingestion, preprocessing, training)
├── utils/                # Helper functions
├── static/               # Web UI styles
├── templates/            # Web UI templates
├── logs/                 # Logging information
├── venv/                 # Virtual environment
├── Dockerfile            # Containerization
├── Jenkinsfile           # CI/CD automation
├── requirements.txt      # Dependencies
└── setup.py              # Package setup
```

## 🔄 Workflow
1. **Data Processing:** Load, clean, and preprocess raw hotel booking data.
2. **Model Training:** Train a LightGBM model and save artifacts.
3. **Web App:** A Flask-based app for real-time predictions.
4. **CI/CD Pipeline:** Automates model training and deployment using Jenkins.
5. **Docker & Deployment:** Containerized using Docker and deployed to Google Cloud Run.

## 🛠️ Getting Started
```bash
# Clone repository
git clone https://github.com/your-repo.git
cd your-repo

# Create virtual environment & install dependencies
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt

# Run Flask App
python application.py
```

## 🎯 Usage
- **Train Model:** `python training_pipeline.py`
- **Run Web App:** `python application.py`
- **Docker Deployment:** `docker build -t hotel-predict . && docker run -p 5000:5000 hotel-predict`

## 🤝 Contributing
Feel free to fork, create pull requests, and report issues!


## 📩 Contact
For inquiries, reach out at: msuraj20@yahoo.com
