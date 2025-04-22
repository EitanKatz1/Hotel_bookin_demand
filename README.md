# Hotel Booking Cancellation Prediction

This project aims to predict hotel booking cancellations using machine learning techniques. The dataset contains records of hotel bookings, including customer details, booking information, and stay details. The target variable is `is_canceled`, which indicates whether a booking was canceled or not.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Models and Evaluation](#models-and-evaluation)
- [Key Insights](#key-insights)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The goal of this project is to build a machine learning model to predict cancellations, enabling hotels to optimize their operations and revenue management. The project includes data preprocessing, feature engineering, model training, and evaluation.

## Dataset
- **Source**: [Kaggle - Hotel Booking Demand Dataset](https://www.kaggle.com/jessemostipak/hotel-booking-demand)
- **Description**: The dataset contains 32 columns and 119,390 rows, including information about bookings, hotels, customers, and stays.

## Project Workflow
1. **Exploratory Data Analysis (EDA)**:
    - Analyzed the dataset structure, missing values, and class distribution.
    - Visualized correlations and seasonal trends.

2. **Data Preprocessing**:
    - Handled missing values and outliers.
    - Balanced the dataset using SMOTE.
    - Scaled numerical features for consistency.

3. **Feature Engineering**:
    - Created new features like `total_guests`, `total_stay`, and `adr_per_person`.
    - Encoded categorical features using one-hot and frequency encoding.

4. **Model Training and Evaluation**:
    - Trained Logistic Regression, Random Forest, Gradient Boosting, and Stacking models.
    - Tuned hyperparameters using GridSearchCV.
    - Evaluated models using metrics like ROC-AUC, precision, recall, and F1-score.

## Models and Evaluation
- **Best Model**: Stacking Model
- **Performance**:
  - ROC-AUC: 0.9533 (after hyperparameter tuning)
  - The Stacking Model outperformed other models, combining the strengths of Logistic Regression, Random Forest, and Gradient Boosting.

## Key Insights
1. **Seasonal Trends**:
    - Higher cancellations during peak months like June and July.
    - Stable bookings in off-peak months like November and December.

2. **Key Features**:
    - `lead_time`, `previous_cancellations`, and `total_of_special_requests` significantly impact cancellations.

3. **Operational Recommendations**:
    - Implement overbooking strategies during peak months.
    - Offer promotions to reduce cancellations.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/hotel-booking-cancellation-prediction.git
    cd hotel-booking-cancellation-prediction
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Run the Jupyter Notebook to explore the analysis and train models:
    ```bash
    jupyter notebook
    ```
2. Use the trained model for predictions:
    - Load the model and input new booking data for predictions.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
