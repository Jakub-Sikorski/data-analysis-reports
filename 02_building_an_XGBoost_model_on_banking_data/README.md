# Bank Deposit Prediction using XGBoost

## Project Description
This project focuses on building an advanced classification model using the XGBoost algorithm to predict whether a client will subscribe to a term deposit. Precise targeting allows banks to optimize operational costs and increase the effectiveness of marketing campaigns. The analysis is based on historical data from direct telemarketing campaigns conducted by a banking institution between May 2008 and November 2010.

## Technologies Used
* **Python**
* **Pandas:** Data cleaning and preprocessing.
* **Scikit-learn:** Data splitting, evaluation metrics, label encoding, and permutation importance.
* **XGBoost:** Core classification algorithm.
* **Scikit-optimize:** Bayesian optimization for hyperparameter tuning.
* **SHAP:** Model explainability and feature importance analysis.
* **Matplotlib:** Data visualization.

## Methodology
The analytical process consists of three main stages:
1. **Exploratory Data Analysis (EDA) & Data Preparation:** Statistical analysis, distribution exploration, multicollinearity checks, and target correlation analysis. The data was split into Train (60%), Validation (20%), and Test (20%) sets.
2. **Model Building & Optimization:** Sequential training of multiple XGBoost models, experimenting with default parameters, dummy variable encoding, and Bayesian hyperparameter optimization. Models were evaluated using the Gini coefficient.
3. **Champion Model Selection & Evaluation:** Selecting the best-performing model based on stability and predictive power, followed by an in-depth evaluation including SHAP values for feature importance.

## Key Findings
* **Exploratory Data Analysis:** The target audience shows a "U-shaped" profile concerning age, with the highest probability of subscription among the youngest and oldest clients, despite less frequent contact with the latter group. Inactive groups (students, retirees) show the highest conversion probability, unlike blue-collar workers and management, who represent the largest volume of contacts but have a lower conversion rate.
* **Model Optimization:** Base models showed a strong tendency to overfit (Gini ~95-97% on Train, dropping significantly on Valid/Test). Full Bayesian optimization on dummy variables also resulted in overfitting.
* **Champion Model:** The hybrid approach proved to be the best. Applying hyperparameters optimized on Label Encoded data to the Dummy variable structure drastically reduced overfitting, achieving high and stable results across Validation and Test sets.

## File Structure
* `lista2.ipynb` - The main Jupyter Notebook containing EDA, model training, optimization, and evaluation.
* `bank-full.csv` - The dataset used for the analysis.
