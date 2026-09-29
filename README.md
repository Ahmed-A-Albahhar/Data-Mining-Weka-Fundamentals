# Data-Mining-Weka-Fundamentals
A foundational data mining project applying Classification (J48), Clustering (K-Means), and Association Rules (Apriori) using Weka.
# Business Intelligence & Data Mining: Weka Algorithmic Analysis

## 📌 Project Overview
This foundational project demonstrates the application of core data mining algorithms using the Weka Explorer environment. Utilizing a standardized environmental dataset featuring 5 key attributes (Outlook, Temperature, Humidity, Windy, and Play), the objective was to extract actionable patterns and predict outcomes using three distinct data mining methodologies: Classification, Clustering, and Association Rule Mining.

## 💡 Key Algorithmic Competencies
Even foundational datasets prove an understanding of how raw data is mathematically segmented to drive business or operational decisions. 
* **Predictive Classification:** Engineered a decision tree to classify optimal conditions, mimicking how businesses predict customer churn or risk.
* **Unsupervised Clustering:** Grouped disparate data points into behavioral clusters, demonstrating the statistical foundations used in market segmentation.
* **Pattern Extraction:** Utilized support and confidence thresholds to extract definitive association rules, the same logic underlying e-commerce recommendation engines and market basket analysis.

## ⚙️ Technical Implementation & Methodologies

### 1. Classification (J48 Decision Tree)
* **Execution:** Processed the data using the J48 Decision Tree algorithm with a 50/50 training and testing split.
* **Outcome:** Generated a pruned decision tree with 8 total nodes and 5 terminal leaves.
* **Logic Flow:** The model established that `Outlook` was the primary splitting criterion; it further classified `Sunny` days by `Humidity`, and `Rainy` days by `Windy` conditions. 
* **Evaluation Metrics:** Validated model performance using standard classification metrics including True Positive (TP) Rate, False Positive (FP) Rate, Precision, Recall, F-Measure, and ROC/PRC Areas.

### 2. Clustering (Simple K-Means)
* **Execution:** Deployed the Simple K-Means algorithm to group the data without predefined labels.
* **Outcome:** The algorithm successfully identified distinct natural groupings, with `Cluster 0` mathematically representing the most common, optimal conditions (Sunny, Mild, High Humidity, Non-Windy).

### 3. Association Rule Mining (Apriori Algorithm)
* **Execution:** Mined the dataset for frequent itemsets using the Apriori algorithm, setting strict parameters of 90% Confidence and 15% Support.
* **Extracted Rules:** 
  * If `Outlook = Overcast`, then `Play = Yes`.
  * If `Outlook = Sunny` AND `Humidity = High`, then `Play = No`.
  * If `Outlook = Rainy` AND `Windy = False`, then `Play = Yes`.
