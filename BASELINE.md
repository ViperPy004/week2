# Baseline Model

## Model
DummyClassifier(strategy='most_frequent') — always predicts "No Churn".

## Metrics
- Accuracy: 0.73
- Precision (Churn=Yes): 0.00
- Recall (Churn=Yes): 0.00
- F1 (Churn=Yes): 0.00

## Why Accuracy Is Misleading
The baseline gets 73% accuracy because 73% of customers stayed. But it catches 0% of churners. For the business, catching churners is the whole point. A model that never predicts churn is useless, even with 73% accuracy.

## Implication
Any real model must beat this on recall and F1 for the churn class. Do not judge future models on accuracy alone.
