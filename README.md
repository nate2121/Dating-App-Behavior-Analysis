# Dating-App-Behavior-Analysis
A full exploratory, modeling, and segmentation study of user behavior on a dating platform. This project analyzes a large-scale dating app behavior dataset to uncover patterns in swiping behavior, match outcomes, engagement levels, and user personas.
It combines exploratory data analysis, feature engineering, machine learning models, and clustering techniques to build a comprehensive understanding of what drives successful matches on dating platforms.

The notebook includes visualizations, statistical summaries, predictive modeling, and segmentation insights that can be used for product optimization, user experience improvements, or behavioral research.

Project Objectives
Understand how users interact with a dating app

Identify behavioral patterns that correlate with higher match success

Engineer meaningful features such as:

Total Interactions

Engagement Score

Selectiveness

Match Rate

Build predictive models to classify High Match Users

Segment users into behavioral personas using clustering

Visualize trends across gender, engagement, swiping behavior, and match outcomes

Dataset Overview
The dataset includes 50,000 user records with features such as:

Gender & age

Swipe right ratio

Mutual matches

Likes received

Messages sent

App usage time

Stress/anxiety indicators (if present)

Engagement metrics

Detects column names using fuzzy matching to ensure flexibility across similar datasets.

  Key Analyses & Visualizations
Exploratory Data Analysis
Mutual matches by gender

Swipe‑right ratio vs. match outcomes

Distribution of matches by app usage time

Engagement score distribution

Correlation heatmap

Feature Engineering
Total_Interactions = messages_sent + likes_received

Engagement_Score = messages_sent (or combined if received messages exist)

Selectiveness = likes_received / swipes

Match_Rate = mutual_matches / swipes

User Segmentation
Using KMeans clustering, users are grouped into personas based on interaction and engagement metrics.

Predictive Modeling
Models trained to classify High Match Users:

Model	Accuracy	AUC
Random Forest	~0.56	~0.586
Logistic Regression	~0.55	~0.593
XGBoost	~0.58	~0.594


Includes:

Classification reports

Feature importance plots

ROC curve comparisons

  Machine Learning Workflow
Data Cleaning

Handle missing values

Replace infinite values

Impute using training‑set means

Train/Test Split

80/20 split

Model Training

Random Forest

Logistic Regression

XGBoost

Evaluation

Accuracy

Precision/Recall/F1

ROC/AUC

Feature importance

Clustering

KMeans (4 clusters)

Persona visualization

Cluster summary table

 Example Insights
Engagement score shows meaningful separation between high‑match and regular users.

Selectiveness varies dramatically across clusters, revealing distinct behavioral personas.

Swipe‑to‑match conversion rates highlight inefficiencies in user behavior.

Gender differences appear in match rate distributions and interaction patterns.

 Technologies Used
Python

Pandas, NumPy

Seaborn, Matplotlib, Plotly

Scikit‑learn

XGBoost

SHAP (for model explainability)

Google Colab

  Acknowledgments
This project was developed as part of a broader exploration into behavioral analytics, machine learning, and data storytelling.
Thanks For Reading!
