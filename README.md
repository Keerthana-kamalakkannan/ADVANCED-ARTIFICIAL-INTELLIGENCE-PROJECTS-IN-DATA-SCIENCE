# ADVANCED-ARTIFICIAL-INTELLIGENCE-PROJECTS-IN-DATA-SCIENCE
'''
============================================================
PROJECT TITLE
Data-Driven Customer Profiling: Financial Behavior Analysis
for Personalized Banking Benefits
============================================================

PROJECT OVERVIEW
This project builds a machine learning system to analyze customer behavior in the banking domain and generate meaningful insights for segmentation and decision-making.

It evaluates:
- Spending behavior
- Response to offers and rewards
- Fraud risk patterns
- Brand and lifestyle preferences

Based on this, customers are grouped into segments such as VIP, Loyal, Impulsive, Risky, and Standard.

------------------------------------------------------------

DEVELOPMENT ENVIRONMENT

The project was initially developed using Google Colab for:
- Data exploration
- Model training and experimentation
- Testing machine learning models in a cloud-based environment

Google Colab was used because it provides easy setup and access to pre-installed libraries without local configuration.

In the later stages, the project was moved to a local environment using Visual Studio Code for:
- Code integration
- Final implementation of models
- Building the Streamlit dashboard
- Organizing the complete project structure

------------------------------------------------------------

SETUP INSTRUCTIONS

1. Install Python (version 3.8 or above)

2. Install required libraries:
   pip install -r requirements.txt

3. We can use Google Colab, which doesn't need any installation or configuration


All dependencies are listed in requirements.txt and can be installed using pip install -r requirements.txt.

------------------------------------------------------------

HOW TO RUN

Step 1:
Run the main Python file:
   python train_model.py

This will:
- Load dataset
- Preprocess data
- Train/load models
- Generate customer scores

Step 2:
Enter Customer ID when prompted to view analysis

Step 3:
Run Streamlit dashboard:
   streamlit run app.py

------------------------------------------------------------

MODELS USED

- Reward Model: predicts response to discounts and cashback offers
- Psychology Model: evaluates spending behavior and financial stress
- Fraud Model: detects risky transaction patterns
- Brand Model: identifies premium and lifestyle preference

Each model outputs a probability score between 0 and 1.

------------------------------------------------------------

DATASET
BANKING_DATASET.csv

- Structured tabular dataset
- Contains customer behavioral and transaction features
- Assumed anonymised or synthetic

------------------------------------------------------------

PRE-TRAINED MODELS

The project uses saved models:
- reward_model.pkl
- psychology_model.pkl
- fraud_model.pkl
- brand_model.pkl

If these are not available, they will be generated automatically
when running the main script.

------------------------------------------------------------

PROJECT STRUCTURE

project-folder/
│
├── data/
│   └── encoded_dataset.csv
│   └── users.csv                  (Store users data)
│
├── models/
│   ├── brand_importance.png
│   ├── brand_model.pkl
│   ├── brand_scaler.pkl
│   ├── fraud_importance.png
│   ├── fraud_model.pkl
│   ├── fraud_scaler.pkl
│   ├── model_contribution.png
│   ├── model_correlation_heatmap.png
│   ├── psychology_importance.png
│   ├── psychology_model.pkl
│   ├── psychology_scaler.pkl
│   ├── reward_importance.png
│   ├── reward_model.pkl
│   ├── reward_scaler.pkl
│   ├── risk_vs_value.png

│
├── app.py                  (Streamlit dashboard)
├── train_model.py                (Main execution file)
├── requirements.txt
├── README.md
│
├── outputs/
│   ├── reports/
│   └── charts/

------------------------------------------------------------

OUTPUTS

Train_model.py
- Customer scores (Reward, Psychology, Fraud, Brand)
- Customer segmentation (VIP, Loyal, Impulsive, Risky, Standard)
- Ranking system
- CSV reports for customers
- Visual charts (bar charts, scatter plots, heatmaps)

app.py
- Role-based login system (Admin vs Analyst access)
- Bank-wide analytics dashboard with customer demographics and risk insights
- Individual customer profiling with behavioural scores, segment classification and rankings

------------------------------------------------------------

REQUIREMENTS

- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib
- seaborn
- streamlit
- joblib

------------------------------------------------------------

AUTHORS

-Keerthana Kamalakkannan
-Flavian Morris John Dominic
-Khushi Ajgaonkar
-Taniya Joseph Joseph Martin

============================================================
'''
