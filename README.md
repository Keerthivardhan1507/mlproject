Student Performance Prediction
📌 Project Overview

This project is an end-to-end Machine Learning pipeline built with Python, Scikit-learn, XGBoost, and Flask to predict student math scores based on features such as writing score, reading score, and other attributes.

It covers the full ML workflow:

Data Ingestion

Data Transformation (preprocessing)

Model Training & Evaluation

Model Deployment using Flask

📂 Project Structure
project/
│── artifacts/                # Stores intermediate artifacts
│   ├── data.csv
│   ├── train.csv
│   ├── test.csv
│   ├── model.pkl             # Trained ML model
│   ├── preprocessor.pkl      # Data preprocessing pipeline
│
│── notebook/
│   └── data/
│       └── stud.csv          # Raw dataset
│
│── src/                      # Source code
│   ├── components/           # Core ML pipeline scripts
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │
│   ├── pipeline/             # Training & prediction pipelines
│   │   ├── train_pipeline.py
│   │   ├── predict_pipeline.py
│   │
│   ├── exception.py          # Custom exception handling
│   ├── logger.py             # Logging utility
│   ├── utils.py              # Helper functions
│
│── templates/                # HTML templates for Flask app
│
│── app.py                    # Flask web app entry point
│── requirements.txt          # Python dependencies
│── setup.py                  # Package setup file
│── README.md                 # Project documentation

⚙️ Tech Stack

Python 3.8+

Pandas, NumPy – Data manipulation

Scikit-learn, XGBoost, CatBoost – Machine learning

Flask – Model deployment

Logging & Custom Exceptions – Debugging and error handling

🚀 Installation

Clone the repository:

git clone https://github.com/Keerthivardhan1507/mlproject.git
cd mlproject


Create & activate virtual environment:

conda create -n student_pred python=3.8 -y
conda activate student_pred


Install dependencies:

pip install -r requirements.txt

📊 Usage
1️⃣ Train the Model

Run the training pipeline to preprocess data & train models:

python src/pipeline/train_pipeline.py

2️⃣ Run Flask App (for Predictions)

Start the web application:

python app.py


Open your browser at http://127.0.0.1:5000/
 to access the UI.

📈 Model Training & Evaluation

Multiple ML algorithms implemented:

Random Forest

Decision Tree

Gradient Boosting

Linear Regression

K-Neighbors Regressor

XGBoost

CatBoost

AdaBoost

Models are evaluated using R² Score and the best model is selected.

📌 Future Improvements

Add Docker support for easy deployment

Deploy model on AWS/GCP/Azure

Integrate CI/CD pipeline

🤝 Contributing

Contributions are welcome! Feel free to open an Issue or submit a Pull Request.

📜 License

This project is licensed under the MIT License.
