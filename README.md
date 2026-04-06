
# Financial Risk Prediction with Explainable AI

Overview
This project builds a hybrid AI system for financial risk assessment using machine learning and generative AI. The system predicts loan approval decisions based on transaction data and generates human-readable explanations for each decision.

The goal is to evaluate how reliable generative AI models are when used for financial reasoning tasks.

Features
- Financial feature engineering from transaction data
- Risk prediction using XGBoost
- Explainable AI using a language model
- Evaluation of both prediction performance and GenAI reliability
- Consistency analysis of LLM outputs

Dataset
The project uses real transaction data from a bank statement dataset.

Key features:
- income
- expense
- risk_ratio

Methodology
1. Data preprocessing and cleaning
2. Feature engineering using rolling transaction windows
3. Training XGBoost model for classification
4. Generating explanations using FLAN-T5
5. Evaluating GenAI outputs against rule-based logic

Results
Machine Learning Model:
- Accuracy: 99.7 percent
- Precision: 98.8 percent
- Recall: 100 percent
- F1 Score: 0.99

Generative AI:
- Alignment with rule-based logic: 30 percent
- Consistency across runs: 100 percent

Key Insight
The generative model produced consistent outputs but showed low alignment with financial logic, highlighting limitations of LLMs in numerical reasoning tasks.

Installation
pip install -r requirements.txt

Usage
1. Open main.ipynb
2. Run all cells in order
3. View predictions and generated explanations

Project Structure
- main.ipynb contains full pipeline
- requirements.txt contains dependencies
- data folder contains dataset

Future Work
- Fine-tune LLM on financial data
- Improve numerical reasoning using hybrid models
- Deploy as a web application

Author
Anish Deshmukh
