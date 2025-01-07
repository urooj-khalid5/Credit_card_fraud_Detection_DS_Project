# Credit_card_fraud_Detection_DS_Project
Data Science Project No 1
# EDA of Credit Card Fraud Detection

This project involves performing Exploratory Data Analysis (EDA) on a credit card transaction dataset to uncover patterns and anomalies associated with fraudulent activities. The dataset is sourced from Kaggle and provides a platform to analyze fraud in financial transactions.

## Dataset
- **Source:** [Credit Card Fraud Detection Dataset on Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Rows:** 284,807
- **Columns:** 31

## Installation and Setup

### Prerequisites
- Python (3.x)
- Libraries: pandas, numpy, matplotlib, seaborn
- Kaggle API credentials (kaggle.json)

### Steps
1. Clone this repository.
2. Place your `kaggle.json` file in the root directory.
3. Run the following commands to install dependencies and download the dataset:

```bash
pip install -q kaggle
mkdir ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
kaggle datasets download -d "mlg-ulb/creditcardfraud"
unzip creditcardfraud.zip
```

## Analysis Questions and Results

### Q1: How many rows and columns are in the dataset?
- **Rows:** 284,807
- **Columns:** 31

### Q2: What are the column names and their data types?
- The dataset includes features such as `Time`, `Amount`, and 28 anonymized PCA features.

### Q3: Are there any missing or null values?
- No missing or null values in the dataset.

### Q4: How many transactions are fraudulent and legitimate?
- **Legitimate transactions:** 284,315
- **Fraudulent transactions:** 492

### Q5: What percentage of transactions are fraudulent?
- **Fraudulent transactions percentage:** 0.17%

### Q6: What are the minimum, maximum, mean, and median values for the `Amount` column?
- **Minimum:** 0.00
- **Maximum:** 25,691.16
- **Mean:** ~88.35
- **Median:** ~22.00

### Q7: What is the maximum transaction amount in the dataset, and is it fraudulent?
- **Maximum amount:** 25,691.16
- **Fraudulent:** No

### Q8: Can we create a bar chart showing the count of fraudulent vs. legitimate transactions?
- A bar chart was created showing the count of both types of transactions, highlighting the significant imbalance.

### Q9: What does the histogram of transaction amounts look like?
- The histogram is right-skewed, with most transactions being of smaller amounts and a few outliers.

### Q10: Can we use a heatmap to visualize the correlation between numerical features?
- Yes, a heatmap was used to visualize correlations, with color intensity indicating the strength and direction of correlations.

## Visualizations
1. **Bar Chart**: Counts of fraudulent and legitimate transactions.
2. **Histogram**: Distribution of transaction amounts.
3. **Heatmap**: Correlation between numerical features.

## Conclusion
This project highlights the significance of exploratory data analysis in detecting patterns and anomalies in credit card transactions. While fraudulent transactions are rare, they can be identified by analyzing distributions and correlations in the data.

## Acknowledgments
- Kaggle for the dataset.
- Scikit-learn, Matplotlib, and Seaborn for the tools used in analysis and visualization.


