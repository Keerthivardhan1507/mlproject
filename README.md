🎯 Student Performance Prediction

Welcome to the Student Performance Prediction repository! This project is an end-to-end Machine Learning pipeline built with Python, Scikit-learn, XGBoost, and Flask to predict student math scores based on features such as reading score, writing score, and other attributes.

## 📌 Table of Contents
- [Introduction](#-introduction)
- [Tech Stack](#️-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [Model Training & Evaluation](#-model-training--evaluation)
- [Future Improvements](#-future-improvements)
- [Contributing](#-contributing)
- [License](#-license)


## 🔎 Introduction

This repository demonstrates a complete ML workflow, including:
- Data ingestion
- Data preprocessing & transformation
- Model training and evaluation
- Model deployment using Flask

## It’s designed as a hands-on project for understanding the lifecycle of an ML application.

⚙️ Tech Stack

- Python 3.8+
- Pandas, NumPy – Data manipulation
- Scikit-learn, XGBoost, CatBoost – Machine learning
- Flask – Model deployment
- Logging & Custom Exceptions – Debugging and error handling
##

## Project Structure

```
project/
│
├── artifacts/          # Intermediate files & models
│   ├── data.csv
│   ├── train.csv
│   ├── test.csv
│   ├── model.pkl       # Trained ML model
│   └── preprocessor.pkl# Data preprocessing pipeline
│
├── notebook/           # Jupyter notebooks
│   └── data/
│       └── stud.csv    # Raw dataset
│
├── src/                # Source code
│   ├── components/     # Core ML pipeline scripts
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/       # Training & prediction pipelines
│   │   ├── train_pipeline.py
│   │   └── predict_pipeline.py
│   │
│   ├── exception.py    # Custom exceptions
│   ├── logger.py       # Logging utility
│   └── utils.py        # Helper functions
│
├── templates/          # HTML templates for Flask
│
├── app.py              # Flask app entry point
├── requirements.txt    # Dependencies
├── setup.py            # Package setup
└── README.md           # Documentation
```

## ⚙️ Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Keerthivardhan1507/mlproject.git
    cd mlproject
    ```

2.  **Create & activate a virtual environment:**
    ```bash
    conda create -n myenv python=3.8 -y
    conda activate myenv
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

---

## 🚀 Usage

1.  **Train the Model:**
    ```bash
    python src/pipeline/train_pipeline.py
    ```

2.  **Run the Application (for Predictions):**
    ```bash
    python app.py
    ```
    
Then open your browser: 👉 http://127.0.0.1:5000/

 ## 📈 Model Training & Evaluation

- Implemented ML models:
- Random Forest
- Decision Tree
- Gradient Boosting
- Linear Regression
- K-Neighbors Regressor
- XGBoost
- CatBoost
- AdaBoost
- Models are compared using R² Score and the best-performing model is selected.

## 📌 Future Improvements

1. Add Docker support for deployment
2. Deploy on AWS/GCP/Azure
3. Integrate CI/CD pipeline

## 🤝 Contributing

1. Contributions are welcome! 🎉
2. Open an Issue
3. Submit a Pull Request

## 📜 License
- This project is licensed under the MIT License.


