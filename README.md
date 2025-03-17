# 🏨 Hotel Reservation Cancellation Prediction

## App
![image](https://github.com/user-attachments/assets/ecca5b11-fbbd-445e-b3df-0d768910e35e)

## 🚀 Project Overview
This project aims to predict whether a hotel booking will be canceled using a Machine Learning Operations (MLOps) pipeline. It integrates **data ingestion, preprocessing, model training, deployment, and a user-friendly web application** for real-time predictions. The model is trained on the [Hotel Reservations Dataset](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset), which includes various booking attributes influencing cancellations.

## 🐂 Project Structure
```
├── artifacts/            # Stored models & processed data
├── config/               # Configuration files (YAML, parameter settings)
├── custom_jenkins/       # CI/CD pipeline setup (Jenkins)
├── notebook/             # Exploratory Data Analysis (EDA) & experimentation
├── pipeline/             # ML pipeline for data preprocessing & training
├── src/                  # Core scripts (ingestion, preprocessing, model training)
├── utils/                # Utility functions for data transformation & logging
├── static/               # Web UI stylesheets
├── templates/            # HTML templates for the web UI
├── logs/                 # Application & model logging
├── venv/                 # Virtual environment setup
├── Dockerfile            # Containerization setup
├── Jenkinsfile           # CI/CD automation pipeline
├── requirements.txt      # Required dependencies
└── setup.py              # Package installation setup
```

## 🔄 MLOps Workflow
1. **Database & Project Setup:** Configure and initialize the required infrastructure.
2. **Data Ingestion & Processing:** Load, clean, and preprocess hotel booking data.
3. **Model Training & Experimentation:** Train a **LightGBM** model with hyperparameter tuning.
4. **Versioning & Tracking:** Maintain data and code versioning for reproducibility.
5. **CI/CD Pipeline:** Automate training, validation, and deployment using **Jenkins**.
6. **Web Application:** Flask-based UI for real-time cancellation prediction.
7. **Deployment:** Containerized with **Docker** and deployed on **Google Cloud Run**.

## 🛠️ Getting Started
### Prerequisites
Ensure you have Python installed (Recommended: Python 3.8+).

```bash
# Clone the repository
git clone https://github.com/SM0311/MLOPS-HOTEL-BOOKING-CANCELLATION.git
cd MLOPS-HOTEL-BOOKING-CANCELLATION

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Flask Application
python application.py
```

## 🎯 Usage
- **Train Model:**  
  ```bash
  python training_pipeline.py
  ```
- **Run Web App Locally:**  
  ```bash
  python application.py
  ```
- **Docker Deployment:**  
  ```bash
  docker build -t hotel-predict .
  docker run -p 5000:5000 hotel-predict
  ```

## ⚙️ CI/CD Automation
This project follows a **CI/CD workflow** using **Jenkins**:
- Automated data ingestion and preprocessing.
- Continuous model training and validation.
- Containerized deployment via **Docker & Google Cloud Run**.

## 📊 Model Performance
The model leverages **LightGBM** for high accuracy and efficiency. Performance metrics include:
- **Accuracy:** 90%+
- **Precision & Recall:** Balanced trade-off for optimal prediction.
- **Feature Importance:** Identifies key booking attributes influencing cancellations.

## 🤝 Contributing
Contributions are welcome! Feel free to **fork** this repository, **create pull requests**, and **report issues**.

## 📩 Contact
For inquiries, reach out via **Email:** msuraj20@yahoo.com
