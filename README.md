```markdown
# Sentiment Detection from Comments

This project detects sentiment (positive, negative, neutral) from text comments using machine learning models. It includes preprocessing, model training, noisy data handling, evaluation, and deployment through a Flask web application.
```

## Project Structure

```
.
├── assets/
│   └── plots/                        # Visualizations and graphs
├── data/
│   ├── processed/                    # Cleaned and prepared datasets
│   └── raw/                          # Original/raw datasets
├── env/                              # Python virtual environment (for local use)
│
├── reports/
│   └── eda_report.txt                # EDA summary report
│
├── src/
│   ├── models/                       # Saved ML models
│   ├── reports/                      # Model training reports/logs
│   ├── 01_preprocess.ipynb           # Data cleaning & text preprocessing
│   ├── 02_model_building_evaluation.ipynb  # Initial model training & evaluation
│   ├── 03_inject_noisy.ipynb         # Simulating noisy labels for robustness testing
│   ├── 04_model_building_noisy.ipynb # Training models with noisy data
│   ├── 05_retraining_models.py       # Retraining and saving final models
│   ├── eda_sentiment_analysis.log    # Log from EDA phase
│   └── model_building.log            # Log from model training phase
│
├── web_app/
│   ├── static/                       # CSS, JS, images for frontend
│   ├── templates/                    # HTML templates (e.g., index.html)
│   └── app.py                        # Flask app for serving predictions
│
├── LICENSE                           # License for the project
├── README.md                         # Project documentation
└── requirements.txt                  # Python dependencies

```

## Features

- Sentiment classification using clean and noisy datasets
- Preprocessing including cleaning, tokenization, and vectorization
- Model training and evaluation with logging
- Web app for real-time predictions using Flask
- EDA and performance visualizations

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/sentiment-detection-comments.git
cd sentiment-detection-comments
```

### Create Virtual Environment

```bash
python -m venv env
```

### Activate Environment

- On Linux/macOS:

```bash
source env/bin/activate
```

- On Windows:

```bash
env\Scripts\activate
```

### Install Requirements

```bash
pip install -r requirements.txt
```

### Run Notebooks

```bash
jupyter notebook src/
```

### Launch Web App

```bash
cd web_app
python app.py
```

## Workflow

- Preprocessing of text data
- Exploratory Data Analysis
- Model building and evaluation
- Noise injection for robustness testing
- Retraining with mixed data
- Deployment with Flask

## Web App Usage

- Enter a comment in the input box
- Click submit to see sentiment prediction
- Backend uses the trained model

## Outputs

- Classification report
- Confusion matrix
- Accuracy and loss plots

## To Do

- Add deep learning model (LSTM, BERT)
- Improve UI of web interface
- Add language support

## License

This project is licensed under the MIT License. See `LICENSE` for details.

## Author

**Shreya Gupta**  
B.Tech CSE, NIT Manipur

