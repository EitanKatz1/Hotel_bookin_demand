# Hotel Booking Demand Analysis & Cancellation Prediction

## Overview

This project focuses on analyzing hotel booking demand data and building a machine learning solution to predict booking cancellations. Hotels face significant revenue loss due to cancellations, making early prediction valuable for resource planning, revenue management, and customer retention strategies.

The dataset contains booking information for both city hotels and resort hotels, including customer demographics, reservation details, booking history, and stay characteristics.

## Key Features

* **Exploratory Data Analysis (EDA)**: Comprehensive analysis of booking patterns, cancellation trends, missing values, correlations, and outliers.
* **Data Cleaning**: Handling missing values and preparing the dataset for analysis.
* **Feature Engineering**: Creation of new features and transformation of categorical variables to improve predictive performance.
* **Correlation Analysis**: Identification of factors most strongly associated with booking cancellations.
* **Cancellation Insights**: Investigation of customer behaviors and booking characteristics that contribute to cancellations.

## Key Findings

* **Lead Time** shows a strong positive relationship with cancellations. Customers who book further in advance are more likely to cancel.
* **Previous Cancellations** increase the likelihood of future booking cancellations.
* **Special Requests** are negatively correlated with cancellations, indicating that engaged customers tend to keep their reservations.
* Certain booking channels, market segments, and room reservation types exhibit different cancellation behaviors.
* Missing values in features such as `agent` and `company` require special handling due to their high proportion.

## Project Workflow

1. **Data Loading**

   * Load and inspect the Hotel Booking Demand dataset.
   * Understand dataset structure and feature distributions.

2. **Exploratory Data Analysis (EDA)**

   * Analyze booking and cancellation patterns.
   * Examine feature distributions and relationships.
   * Visualize correlations and trends.

3. **Data Cleaning**

   * Identify and handle missing values.
   * Remove or address anomalies and inconsistencies.

4. **Feature Engineering**

   * Select relevant features.
   * Encode categorical variables.
   * Create additional predictive features.

5. **Data Preparation**

   * Prepare data for machine learning.
   * Split data into training and testing sets.

6. **Model Development**

   * Build predictive models for cancellation prediction.
   * Evaluate performance using appropriate classification metrics.

## Dataset

The dataset is publicly available on Kaggle:

**Hotel Booking Demand Dataset**

The dataset contains approximately **119,000 hotel bookings** with **32 features**, including:

* **hotel**: Type of hotel (City Hotel or Resort Hotel)
* **lead_time**: Number of days between booking and arrival
* **arrival_date** features
* **stays_in_weekend_nights**
* **stays_in_week_nights**
* **adults**, **children**, **babies**
* **meal**
* **country**
* **market_segment**
* **distribution_channel**
* **reserved_room_type**
* **booking_changes**
* **previous_cancellations**
* **previous_bookings_not_canceled**
* **customer_type**
* **adr** (Average Daily Rate)
* **is_canceled** (Target Variable)

### Target Variable

* **0** → Booking was not canceled
* **1** → Booking was canceled

## Tools and Libraries

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/Hotel_Booking_Demand.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Hotel_Booking_Demand
   ```

3. Install required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open:

   ```bash
   Hotel_bookin_demand_EDA.ipynb
   ```

6. Run all cells sequentially to reproduce the analysis.

## Visualizations

The project includes:

* Correlation heatmaps
* Missing value analysis
* Feature distribution plots
* Cancellation trend visualizations
* Outlier detection plots

## Business Impact

Accurate cancellation prediction enables hotels to:

* Improve occupancy forecasting.
* Optimize pricing strategies.
* Reduce revenue loss from cancellations.
* Improve resource allocation and staffing decisions.
* Develop targeted retention campaigns for high-risk bookings.

## Conclusion

This project demonstrates how exploratory data analysis and feature engineering can uncover valuable insights into hotel booking behavior. Understanding the factors that influence cancellations helps hotels make data-driven decisions and provides a strong foundation for developing predictive machine learning models.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
