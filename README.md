# Customer-Churn-Prediction
This repository implements a Customer Churn Prediction System for **ConnectTel**, addressing churn's impact on business growth. Using machine learning, it identifies at-risk customers, enabling targeted retention. It includes EDA, feature engineering, model training, evaluation, and documentation to enhance retention, loyalty, and profitability.

![image](https://github.com/user-attachments/assets/de0bb897-b9fd-4255-a909-1c4d4d03ba5b)

This project tackles the critical challenge of customer churn faced by ConnectTel, a leading telecommunications company. By employing advanced machine learning techniques, it predicts at-risk customers and provides actionable insights for targeted retention strategies, ultimately improving customer loyalty and driving business growth.

## Project Objectives
The key objectives of this project are:
- **Identify At-Risk Customers**: Predict customers likely to churn based on historical data.
- **Improve Customer Retention**: Implement proactive, personalised interventions to reduce churn.
- **Optimise Marketing Spend**: Target resources effectively for maximum return on investment.
- **Gain Insights into Churn Drivers**: Understand factors influencing customer churn to improve services.
- **Enhance Long-Term Loyalty**: Strengthen customer relationships to sustain business growth.

## Dataset Description
The dataset includes the following key attributes:
- **Demographics**: Gender, Senior Citizen, Partner, Dependents.
- **Service Details**: Phone Service, Multiple Lines, Internet Service, Online Security, etc.
- **Account Information**: Tenure, Contract Type, Payment Method, Monthly Charges, Total Charges.
- **Target Variable**: Churn status indicating if a customer has left or stayed.

## Exploratory Data Analysis (EDA)
Key findings from the EDA:
- Customers with **month-to-month contracts** have significantly higher churn rates.
- **Senior citizens** and customers with **high monthly charges** are more likely to churn.
- Retention improves as customer tenure increases, highlighting the importance of engaging new customers early.
- Lack of add-on services, such as online security and device protection, is linked to higher churn.

## Feature Engineering
- Created **tenure groups** to categorise customers by their duration with ConnectTel.
- Dropped irrelevant or multicollinear features, such as `CustomerID` and `Tenure`.
- Categorical variables were encoded, and synthetic samples were generated using **SMOTEENN** for class balance.

## Machine Learning Models
The following models were tested:
1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **SGDClassifier**
5. **XGBClassifier**

### Best Model: XGBClassifier with SMOTEENN
- **Training Recall**: 99%
- **Test Recall**: 97%
- High precision and recall ensure accurate predictions while minimising false positives and negatives.
- Feature importance and interpretability analysed using **SHAP**.

## Recommendations
Based on insights from the analysis:
1. **Develop Targeted Retention Strategies**: Focus on at-risk customers based on model predictions.
2. **Improve Service Offerings**: Address issues like lack of add-ons and high monthly charges.
3. **Optimise Marketing Spend**: Allocate resources to retention efforts with the highest impact.
4. **Continuous Monitoring**: Regularly evaluate and update the model to maintain effectiveness.

## Repository Structure
- **`data/`**: Contains the dataset used for the analysis.
- **`notebooks/`**: Jupyter Notebooks for EDA, feature engineering, and model training.
- **`scripts/`**: Python scripts for preprocessing, model training, and evaluation.
- **`reports/`**: Generated analysis reports and visualisations.
- **`models/`**: Saved machine learning models.
- **`README.md`**: This file.

## How to Use

1. **Clone this Repository**:  
   Open a terminal or command prompt and run the following commands to download the repository:
   ```bash
   git clone https://github.com/enniej/Customer-Churn-Prediction.git
   cd Customer-Churn-Prediction
2. **Set up the Environment**:
Install the required Python libraries by running:
   ```bash
    pip install -r requirements.txt

3. Explore the Dataset:
Navigate to the `data/` folder to view the dataset used for this project. Ensure you have permission to use or view the dataset.

4. Run Jupyter Notebooks:
Open the Jupyter Notebooks located in the `notebooks/` folder to replicate the steps for:
Exploratory Data Analysis (EDA)
Feature Engineering
Model Training and Evaluation
Start the Jupyter Notebook server using:
   ```bash
   jupyter notebook

## Conclusion
This project provides a robust, data-driven solution for mitigating customer churn at ConnectTel. It combines advanced analytics and machine learning to offer actionable insights and effective strategies for improving customer retention and strengthening ConnectTel's market position.

   
