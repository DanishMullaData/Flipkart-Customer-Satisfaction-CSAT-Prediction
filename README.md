# Flipkart-Customer-Satisfaction-CSAT-Prediction

Machine learning classification project built for the AlmaBetter Data Science capstone.

## Problem
Flipkart collects a satisfaction score (CSAT, 1 to 5) after each customer support interaction. The goal is to predict this score from the details of the support ticket, so Flipkart can find what drives customer satisfaction and improve its service.

## Dataset
`Customer_support_data.csv`, provided by AlmaBetter. It is not included in this repo.

## Approach
1. Explored the data: columns, CSAT distribution, missing values
2. Cleaned the data and parsed dates in day-first format
3. Removed a target leak (`is_satisfied`), which was effectively the answer
4. Dropped high-cardinality columns (`Customer_City`, `Agent_name`) before encoding
5. Encoded categorical features
6. Trained and tuned models, and picked the best one

## Result
Tuned Gradient Boosting model with about **65.8% accuracy** on the 5-class CSAT target (random guessing would give about 20%).

## Files
- `Module_5_ML_Submission_Danish (5).ipynb`: full notebook with code, outputs and written answers

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Google Colab

## Author
Danish Mulla | [LinkedIn](https://linkedin.com/in/danishbest) | [GitHub](https://github.com/DanishMullaData)
