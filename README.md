# Credit_Card_Fraud_Classification

🕵️‍♂️ Credit Card Fraud Detection with Unsupervised Learning
This project aims to detect potentially fraudulent credit card transactions using unsupervised learning techniques. Traditional fraud detection systems often struggle to keep up with evolving patterns — this project addresses that by identifying anomalous behavior without needing labeled data.

🚀 Problem Statement
Company ABC, a major credit card provider, faces delays in identifying new fraud patterns, resulting in significant financial losses. They've provided anonymized transaction and cardholder data to design an intelligent system capable of flagging unusual activities for further investigation.

📁 Dataset
The project uses two CSV files:

cc_info.csv: Contains general credit card and cardholder data (e.g., city, state, credit limit)

transactions.csv: Logs of credit card transactions (date, amount, geolocation)

📊 Key Features Engineered
Transaction-to-Credit Limit Ratio

Transaction Hour

Daily Total Spent per Card

Z-Score of Transaction Amount per Card

Transaction Count per Card

These features help capture behavioral patterns and detect deviations that may indicate fraud.

🧠 Models Applied
Four unsupervised anomaly detection algorithms were implemented and compared:

KMeans Clustering (distance from centroid + smallest cluster)

DBSCAN (density-based anomaly detection)

Local Outlier Factor (LOF)

Isolation Forest

Anomalies were identified using both cluster memberships and outlier scores.

📈 Evaluation Approach
Since this is an unsupervised problem (no ground-truth fraud labels), model performance was assessed based on:

Anomaly score distributions

Statistical characteristics of flagged transactions

Consensus across models (ensemble-style voting)

Manual inspection of top outliers

🔍 Future Work
Add labeled data or conduct expert review

Use geospatial features (e.g., transaction distance from home)

Implement advanced models like Autoencoders or HDBSCAN

Create interactive dashboards with Plotly or Streamlit

Turn this into a real-time fraud scoring pipeline

📌 Tools Used
Python, pandas, scikit-learn, matplotlib

Jupyter Notebooks for development and analysis
