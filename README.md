# Heart Stroke Prediction System

![image alt](https://github.com/MostafaAI10/VisualScribe-Image-Captioning-CNN-LSTM/blob/8cc798c134312a4669c8e93f8ed05ad4a7b67c6e/visualscribe_banner.png)

An end-to-end MLOps-powered healthcare platform for predicting stroke risk using machine learning, real-time APIs, workflow orchestration, monitoring, and interactive web applications.

## Overview

Heart Stroke Prediction System is a comprehensive machine learning solution designed to assist healthcare professionals in assessing a patient's risk of stroke based on clinical and demographic information. By leveraging predictive analytics, the system provides risk assessments that can support early intervention and informed medical decision-making.

Users can enter patient health information through a user-friendly web interface or integrated medical devices. The trained machine learning model then analyzes the provided data and generates a stroke risk prediction along with actionable insights, recommendations, and precautionary guidance.

---

## 🎯 Target Users

* Healthcare Professionals
* Doctors & Medical Practitioners
* Clinics & Hospitals
* Medical Device Integrators
* Healthcare Researchers

---

## ✨ Key Features

### 1: Interactive Web Application

Built with **Streamlit** to provide an intuitive interface for patient data entry, prediction visualization, and result interpretation.

### 2: High-Performance Prediction API

Powered by **FastAPI**, enabling scalable and efficient prediction services for external applications and healthcare systems.

### 3: Machine Learning Model Package

A production-ready Python package (`stroke-pred-p0w11`) trained to predict stroke probability using clinical indicators.

### 3: Data Management Layer

Utilizes **PostgreSQL** and **SQLAlchemy** for reliable data storage, management, and persistence.

### 4: Automated Data Ingestion Pipeline

Implemented with **Apache Airflow** to automate data collection, processing, and workflow orchestration.

### 5: Prediction Monitoring & Observability

Integrated with **Grafana** dashboards for monitoring prediction metrics, system performance, and operational insights.

---

## 🏗️ System Architecture

```text
User Input
    │
    ▼
Streamlit Web Interface
    │
    ▼
FastAPI Prediction Service
    │
    ▼
Machine Learning Model
    │
    ├── Store Results → PostgreSQL
    │
    └── Monitor Metrics → Grafana

Airflow
    │
    └── Data Ingestion & Pipeline Automation
```

![Screenshot 2022-04-27 at 6 56 27 PM](https://github.com/MostafaAI10/Heart-Stroke-Prediction/blob/92badced2051c74103c2e4ad840dd785c47c0675/heart_stroke_prediction/DSP.drawio.png)

---

## 📊 Dataset

The model is trained using the Stroke Prediction Dataset containing 11 clinical and demographic features associated with stroke risk.

Dataset Source:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

Features include:

* Gender
* Age
* Hypertension
* Heart Disease
* Marital Status
* Work Type
* Residence Type
* Average Glucose Level
* BMI
* Smoking Status
* Additional demographic attributes

---

## 🛠️ Technology Stack

| Component              | Technology           |
| ---------------------- | -------------------- |
| Frontend               | Streamlit            |
| Backend API            | FastAPI              |
| Machine Learning       | Python, Scikit-Learn |
| Database               | PostgreSQL           |
| ORM                    | SQLAlchemy           |
| Workflow Orchestration | Apache Airflow       |
| Monitoring             | Grafana              |
| Containerization       | Docker (Optional)    |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <github.com/MostafaAI10/Heart-Stroke-Prediction/tree/main>
cd stroke_heart_prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

For macOS/Linux users:

```bash
pip install psycopg2-binary
```

---

## ⚙️ Environment Configuration

Create a `.env` file in the project root:

```env
POSTGRES_USER=your_username
POSTGRES_PASSWORD=your_password
POSTGRES_SERVER=localhost
POSTGRES_PORT=5432
POSTGRES_DB=stroke_prediction

BACKEND_SERVER=http://localhost:8005
```

---

## 🗄️ Database Setup

Navigate to the PostgreSQL module:

```bash
cd postgres
python createdb.py
```

This will automatically create the required tables and database relationships.

---

## Airflow Setup

Follow the instructions provided in the Airflow documentation inside the repository.

**AirFlow Setup:** [AirFlow](https://airflow.apache.org/)

---

## Grafana Dashboard

Follow the Grafana setup guide available in the repository to configure monitoring and visualization dashboards.

**Grafana:** [Get Started](https://grafana.com/)

---

## ▶️ Running the Application

### Start FastAPI Backend

```bash
cd stroke_api

uvicorn main:app \
--host 0.0.0.0 \
--port 8005
```

### Launch Streamlit Interface

```bash
streamlit run web_interface.py --server.port 8010
```

---

## 🌟 Project Goals

* Enable early stroke risk detection.
* Support healthcare professionals with AI-assisted decision making.
* Demonstrate production-grade MLOps practices.
* Provide scalable deployment and monitoring capabilities.
* Bridge machine learning research with real-world healthcare applications.

---

## ⚠️ Disclaimer

This project is intended for educational, research, and decision-support purposes only. Predictions generated by the system should not replace professional medical diagnosis, treatment, or consultation.

---

## Contact Information

**MOSTAFA ABDELHAMED**

Email: [abdelhamedmostafa190@gmail.com](mailto:abdelhamedmostafa190@gmail.com)

---

## Acknowledgements

Special thanks to the open-source community and contributors whose tools and research made this project possible. Your work continues to inspire innovation in AI-driven healthcare solutions.

---



