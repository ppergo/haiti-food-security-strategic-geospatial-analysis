Advanced Predictive Modeling for Human Behavior Analysis
A Portfolio Project Demonstrating Techniques Beyond a Standard Curriculum

[Project Status: Complete]

1. Strategic Context: From Corporate Data to Humanitarian Insight
This project uses a classic "Employee Churn" dataset not as an end in itself, but as a methodological case study to demonstrate a transferable analytical framework. The core challenge—understanding and predicting human behavior based on structured data—is universal and directly applicable to critical questions in the humanitarian and development sectors.

The methodology developed here can be immediately adapted to:

📈 Predict Vulnerability: The same techniques used to identify employees at risk of leaving can be used to model the risk of a household falling into food insecurity or a beneficiary dropping out of a livelihood program.

📊 Analyze Beneficiary Feedback: This project provides a blueprint for deep analysis of survey data (e.g., PDM, baseline/endline studies). It moves beyond simple descriptive statistics to uncover the complex drivers behind beneficiary satisfaction, program success, or failure.

🎯 Optimize Resource Allocation: The ultimate goal of this analysis is to enable targeted interventions. This mirrors the core task of humanitarian targeting: using data to direct limited resources to the people who need them most, maximizing impact and efficiency.

2. Project Approach: Beyond the Google Analytics Certificate
While this project utilizes the "Salifort Motors" dataset from the Google Advanced Analytics Certificate, it intentionally expands beyond the curriculum's scope to serve as a comprehensive portfolio piece. The analysis within the accompanying notebook showcases a more advanced and robust machine learning workflow, demonstrating proficiency in techniques critical for real-world applications.

Key advanced elements featured in this analysis include:

Statistical Hypothesis Testing in EDA: Applying formal statistical tests (e.g., Shapiro-Wilk, Levene's test, Mann-Whitney U test) to rigorously validate insights from data visualization, adding a layer of statistical certainty to the exploratory phase.

Rapid Multi-Model Baselining: Using LazyClassifier to quickly evaluate the performance of over 20 classification algorithms, providing a data-driven foundation for model selection.

Advanced Correlation Analysis: Employing libraries like Dython and Xicorpy to capture not only linear but also complex non-linear relationships between variables.

Sophisticated Imbalance Handling: Implementing techniques from the imbalanced-learn library to effectively address class imbalance, a common challenge that often degrades model performance.

Performance Optimization: Leveraging the Intel® Extension for Scikit-learn (scikit-learn-intelex) to accelerate model training and prediction, demonstrating an awareness of computational efficiency.

Robust Feature Engineering and Hyperparameter Tuning: Going beyond basic feature creation to develop and test hypotheses, followed by systematic optimization of the chosen model (XGBoost).

3. Case Study Methodology: The PACE Framework
The project follows the PACE (Plan, Analyze, Construct, Execute) framework, a structured methodology for data science projects.

PLAN: Project Scoping and Definition

Objective: Build and validate a machine learning model that accurately predicts employee churn, with a primary focus on maximizing Recall to minimize missed cases.

ANALYZE: Deep Data Exploration

This phase includes advanced data profiling, statistical validation, and creating visualizations to uncover deep-seated drivers of churn.

CONSTRUCT: Advanced Model Development

This phase involves the advanced techniques mentioned above: multi-model evaluation, feature engineering, handling class imbalance, and fine-tuning high-performance models like XGBoost.

EXECUTE: Reporting and Strategic Recommendations

The final phase focuses on summarizing key findings, presenting the final model's performance, and providing actionable strategic recommendations to support proactive interventions.

4. Technical Implementation
Installation
The analysis leverages a powerful set of libraries. Ensure they are installed in your Python environment:

Bash

pip install pandas numpy matplotlib seaborn lazypredict diptest dython xgboost scikit-learn-intelex imbalanced-learn xicorpy
Usage
Clone the repository or download the source files.

Ensure you have the HR_dataset.csv file in the same directory as the notebook.

Open and run the ML Employee Churn Prediction.ipynb notebook in a Jupyter environment. The notebook is structured to guide you through the entire advanced workflow.

Results
The primary success criterion for this project is the model's Recall score. The notebook details the process of building, training, and evaluating several classification models to identify the one that best minimizes False Negatives. The final model serves as a powerful and reliable tool for proactive retention, acting as a blueprint for similar intervention-focused models in other domains.
