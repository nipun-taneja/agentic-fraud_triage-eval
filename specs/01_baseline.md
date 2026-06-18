# Spec 01 - Baseline fraud model (arching)

## Goal 
Create a fast baseline fraud model that takes in transaction and identity data and ouptus a fraud score per transaction
between 0 to 1 along with its evaluation metrics. 

## Decisions
1. XGBoost is fast the latency would be low.
2. This would serve as baseline to compare train and evaluate the agentic framework.

## Sub Specs
[] 01a_eda.md           - understand the data(eda, fraud rate, data quality stats)  
[] 01b_features.md      - solve for class imbalance, sampling,train test split, feature importance           
[] 01c_train_eval.md    - train and eval mode and run some basic optimisation and persist metrics

## Not in Scope
- data streaming
- over optimisizing model, pick the standard defaults hyperparameters
