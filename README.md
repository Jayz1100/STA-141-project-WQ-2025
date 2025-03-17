# STA-141-project-WQ-2025
utilizes R studio to process neural data from 18 sessions and two test sets (test1, test2), analyzing mice’s decision-making under visual stimuli(2019,Steinmetz)
# README

This repository contains R code for a **neural data analysis** project from the STA 141 course. The key steps include:

1. **Data Loading**  
   - Iterates through 18 session files and two test sets (test1, test2), reading each RDS file into memory.

2. **Data Integration**  
   - Aggregates spike data at both region-level (summing spikes per brain region) and bin-level (average spikes across 40 time bins).

3. **Exploratory Data Analysis (EDA)**  
   - Visualizes success rates, neuron spike distributions, and potential differences across sessions.

4. **Feature Engineering**  
   - Transforms relevant columns (e.g., session ID, contrast differences, time bins) into a design matrix for modeling.

5. **Modeling & Evaluation**  
   - Trains multiple classifiers (XGBoost, Random Forest, SVM, Logistic Regression) on an 80/20 train–test split.
   - Generates predictions for each model and computes metrics such as Accuracy, Confusion Matrix, and AUC.

6. **Session-Specific & Test-Set Analysis**  
   - Tests each model on individual sessions (e.g., Session 1, Session 18) and newly released test data, comparing performance differences.

## Usage
- Open the `.Rmd` file or `.R` scripts to run individual steps (data loading, EDA, modeling).
- Adjust hyperparameters and thresholds in the modeling sections to refine predictions.
- Use additional plotting/analysis functions to explore specific questions or sessions.

## Dependencies
- **R** (version ≥ 4.0)
- Packages: **tidyverse**, **ggplot2**, **dplyr**, **caret**, **xgboost**, **randomForest**, **pROC**

## License
This project is provided for educational purposes. Please consult the course guidelines for usage and citation.
