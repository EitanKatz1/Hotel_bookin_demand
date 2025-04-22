# Fraud Detection in Credit Card Transactions

## Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The dataset used contains transactions made by European cardholders in September 2013. The dataset is highly imbalanced, with only 0.17% of transactions being fraudulent.

## Key Features
- **Exploratory Data Analysis (EDA)**: Insights into the dataset, including class distribution, correlation analysis, and temporal patterns.
- **Feature Engineering**: Creation of new features such as the hour of the day and fraud aggregation by time.
- **Data Preprocessing**: Handling class imbalance using SMOTE and applying standard scaling for normalization.
- **Model Training and Evaluation**: Comparison of three models - Logistic Regression, Random Forest, and Gradient Boosting - to identify the best-performing model.

## Results
- The **Random Forest** model achieved the best performance with the highest accuracy, precision, recall, and F1 score.
- Evaluation metrics and confusion matrices were used to assess model performance.

## Project Workflow
1. **Data Loading**: Load and inspect the dataset.
2. **EDA**: Analyze the dataset to understand patterns and distributions.
3. **Feature Engineering**: Create new features to enhance model performance.
4. **Data Preprocessing**: Handle class imbalance and scale features.
5. **Model Training**: Train and evaluate multiple machine learning models.
6. **Model Selection**: Identify the best-performing model based on evaluation metrics.

## Tools and Libraries
- **Python**: Programming language used for the project.
- **Pandas**: Data manipulation and analysis.
- **Seaborn & Matplotlib**: Data visualization.
- **Scikit-learn**: Machine learning models and evaluation metrics.
- **Imbalanced-learn**: Handling class imbalance using SMOTE.

## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Fraud_Credit_Card.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Fraud_Credit_Card
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Open the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
5. Run the cells sequentially to reproduce the analysis and results.

## Dataset
The dataset used in this project is publicly available and contains anonymized credit card transaction data. It includes 31 features:
- **Time**: Seconds elapsed between the transaction and the first transaction in the dataset.
- **Amount**: Transaction amount.
- **Class**: Target variable (1 for fraud, 0 for non-fraud).
- **V1-V28**: Principal components obtained using PCA.

## Conclusion
The project demonstrates the importance of handling class imbalance and the effectiveness of ensemble methods like Random Forest in fraud detection tasks. The Random Forest model was identified as the most reliable model for detecting fraudulent transactions.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
