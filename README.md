# AI-Based Request Classification and Priority Prediction System

An intelligent machine learning solution designed to automate service request classification, priority prediction, and resolver group assignment for enterprise support operations. The platform analyzes historical service records, applies advanced machine learning models, and predicts request categories, priority levels, and routing information to reduce manual effort, improve operational efficiency, and accelerate incident resolution.

## 🚀 Key Features

* **Automated Request Classification**: Classifies incoming service requests into predefined categories using supervised machine learning models.
* **Priority Prediction**: Predicts ticket priority levels based on request descriptions, historical patterns, and operational attributes.
* **Resolver Group Recommendation**: Recommends the most appropriate resolver group for faster request assignment and reduced manual routing.
* **Advanced Feature Engineering**: Implements preprocessing pipelines for text cleaning, categorical encoding, missing value handling, and feature transformation.
* **REST API Integration**: Exposes prediction services through FastAPI endpoints for seamless integration with enterprise ITSM platforms.
* **Experiment Tracking**: Supports model versioning, experiment tracking, and performance comparison using MLflow.
* **Scalable Architecture**: Built with a modular architecture that supports continuous model improvement and enterprise deployment.

## 🛠️ Tech Stack

* **Programming Language**: Python 3.11
* **Machine Learning**: Scikit-learn, XGBoost
* **Data Processing**: Pandas, NumPy
* **Database**: SQL
* **API Framework**: FastAPI
* **Experiment Tracking**: MLflow
* **Deployment**: REST APIs

## 🚦 Getting Started

### Installation

```bash
# Clone the repository
git clone <repository-url>

# Navigate to project directory
cd ai-request-classification-system

# Create virtual environment
python -m venv venv

# Activate virtual environment
# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### Running the Application

Start the FastAPI application using:

```bash
uvicorn app.main:app --reload
```

The API will be available at:

```text
http://localhost:8000
```

Swagger Documentation:

```text
http://localhost:8000/docs
```

## ⚙️ Configuration

The application configuration is managed using environment variables and configuration files.

Typical configurable parameters include:

* Database Connection
* Model Path
* MLflow Tracking URI
* Logging Configuration
* Prediction Thresholds
* API Settings

Configuration can be stored in:

* `.env`
* `config.yaml`

allowing easy deployment across development, testing, and production environments.

## 🧪 Model Evaluation

The system evaluates machine learning performance using multiple classification metrics, including:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix

Cross-validation and hyperparameter tuning are performed to improve prediction accuracy and model generalization before deployment.

## 🛡️ License

This project is licensed under the Apache-2.0 License.
