# earthquake_damage_prediction.ipynb-
This project focuses on predicting building damage levels caused by earthquakes using machine learning algorithms such as Logistic Regression, Random Forest, and XGBoost. It includes data preprocessing, model evaluation, and Power BI dashboards for visualization of accuracy and regional insights.

**PROJECT OVERVIEW**

This project focuses on predicting building damage levels caused by earthquakes using machine learning algorithms such as Logistic Regression, Decision Tree, Random Forest, and XGBoost.
It aims to classify the extent of damage (Grade 1–3) for each building based on structural and geospatial data.
All insights and model results are visualized using Power BI dashboards for better understanding and regional comparison.

**FILES IN THE PROJECT**                                     
Earthquake_Damage_Prediction.ipynb -  Jupyter Notebook with full ML workflow —preprocessing, training, and evaluation
feature_importance.csv - Combined feature importance results from all models
predictions.csv  -  Predicted damage grades for buildings
final_predictions_for_dashboard.csv - Clean dataset used in Power BI dashboard
Dashboard.pbix - Power BI dashboard showing accuracy, feature importance,and regional damage.

**Dataset Source**

Earthquake Damage Assessment Dataset (Kaggle).

**PROJECT STEPS**

Data Cleaning: Removed missing, inconsistent, and duplicate values.
Feature Engineering: Encoded categorical variables and normalized numerical columns.
Model Training: Implemented Logistic Regression, Decision Tree, Random Forest, and XGBoost.
Evaluation: Compared models using Accuracy, F1 Score, and Cross-validation metrics.
Feature Importance: Identified most influential attributes using model-based ranking.
Visualization: Created interactive Power BI dashboard to visualize regional accuracy and predictions.

**MODEL HIGHLIGHTS**
Model	                   Accuracy	      F1-Macro
Logistic Regression	      0.57	           0.33
Decision Tree	            0.63	           0.57
Random Forest            	0.70	           0.61
XGBoost (Best)	          0.72	           0.64

**KEY OBSERVATIONS**

XGBoost provided the best performance with 72% accuracy.
Features like age, geo_level_1_id, foundation_type, and roof_type had high predictive value.

**POWER BI DASHBOARD**

Visualized:
Accuracy by Region
Damage Grade Distribution (1–3)
Feature Importance Comparison
Geo-level (1, 2, 3) Analysis
Building Age vs Damage Correlation

“This dashboard provides a clear regional overview of building vulnerability and model accuracy, helping interpret which factors contribute most to structural damage after an earthquake.”

**HOW TO RUN**
1.Clone this repository
git clone https://github.com/ravaliamaraj13/Earthquake-Damage-Prediction.git
cd Earthquake-Damage-Prediction

2.Install dependencies:
pip install -r requirements.txt

3.Run all cells — it will generate prediction CSV files.

**Open Power BI Dashboard**
Open Dashboard.pbix in Power BI Desktop.
Refresh data connections to view updated accuracy and regional insights.

**FUTURE WORK**

1.Integrate real-time earthquake data for dynamic risk prediction.
2.Implement Deep Learning models (e.g., LSTM, CNN) for structural damage forecasting.
3.Add additional features like soil type, material cost, and environmental data for improved accuracy.
