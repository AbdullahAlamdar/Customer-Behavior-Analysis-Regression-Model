# Customer Behavior Analysis Models

This project is part of the **Intro to Data Science** course, focusing on analyzing and predicting customer behavior in the electronics section. Using a provided dataset, we explore various machine learning models, including **Linear Regression**, **Decision Tree Classification**, and **K-Means Clustering**.

## Repository Contents

- **Jupyter Notebook**: Includes code for building and evaluating the models.
- **Dataset**: Preprocessed electronics data for analysis.
- **Report**: Detailed comparison of model performances and actionable insights.

## Dataset Overview
The dataset contains 1,000 entries and 23 columns with features such as:
- **Demographics**: `Age`, `Gender`, `Income_Level`
- **Transaction Details**: `Purchase_Amount`, `Purchase_Frequency_Per_Month`
- **Categorical Variables**: `Product_Category`, `Brand`
- **Encoded Features**: `Season_Spring`, `Season_Summer`, etc.
- **Target Variable**: `Will_Purchase_Next_Month` (binary)

### Example Columns:
| Column                         | Description                          |
|--------------------------------|--------------------------------------|
| `Age`                          | Standardized customer age            |
| `Purchase_Amount`              | Standardized purchase amount         |
| `Will_Purchase_Next_Month`     | Target: 1 if the customer will purchase next month, 0 otherwise |

### Preprocessing:
- Missing values in `Customer_ID`, `Gender`, and `Income_Level` were addressed.
- Standardization applied to numerical columns.
- Dummies created for seasonal variables.

## Project Workflow

### 1. Linear Regression
- **Goal**: Predict `Purchase_Amount` based on input features.
- **Performance Metric**: R² (0.90).
- **Strengths**: Simplicity and interpretability.
- **Limitations**: Struggles with non-linear relationships and outliers.

### 2. Decision Tree Classification
- **Goal**: Classify customers likely to make a purchase next month.
- **Performance Metrics**:
  - Precision: 0.75
  - Recall: 0.75
  - F1 Score: ~0.75
- **Strengths**: Captures non-linear patterns and is interpretable.
- **Limitations**: Prone to overfitting without proper tuning.

### 3. K-Means Clustering
- **Goal**: Segment customers into behavioral clusters.
- **Method**: Elbow method to find optimal clusters (k = 4).
- **Insights**: Segments provide actionable insights for targeted marketing.

## Key Findings
- **Targeted Marketing**: Decision trees identified customer segments for personalized offers.
- **Customer Segmentation**: K-Means revealed behavioral clusters aiding in tailored campaigns.
- **Predictive Insights**: Linear regression predicted spending trends for inventory management.

## Actionable Recommendations
- Implement **personalized promotions** using segmentation insights.
- Use regression trends for **inventory forecasting**.
- Explore advanced models (e.g., Random Forest, XGBoost) to enhance predictions.

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/Customer-Behavior-Analysis-Models.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Run the cells sequentially.

## Authors
- **M. Abdullah Alamdar** (23i2597)
- **Romaan Khawar** (23i2554)

## License
This project is licensed under the MIT License.
