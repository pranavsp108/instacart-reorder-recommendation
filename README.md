# Scalable Grocery Reorder Prediction & Basket Recommendation System

## 1. Business Problem
Predict which products a customer is likely to reorder in their next grocery basket.

## 2. Dataset
Instacart order, product, aisle, department, and reorder history.

## 3. Why Scalability Matters
The raw order-product dataset contains 32M+ rows, making naive pandas joins and one-hot market basket encoding inefficient.

## 4. Architecture
Raw CSV → Bronze tables → Silver joined tables → Gold feature tables → ML models → Recommendations

## 5. Feature Engineering
User, product, user-product, and order-context features.

## 6. Leakage Prevention
Features are computed only from orders before the target order.

## 7. Modeling
Logistic Regression baseline, Spark ML tree model, threshold tuning, top-K ranking.

## 8. Evaluation
F1, PR-AUC, Precision@K, Recall@K.

## 9. Market Basket Analysis
Spark FP-Growth association rules for cross-sell recommendations.

## 10. Business Insights
Personalized reorder reminders, department-level cross-sell, customer segment strategy.

## 11. Future Work
Real-time serving, streaming basket updates, A/B testing framework.
