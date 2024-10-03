# Predicting Engagement - What drives ad performance?

This Jupyter Notebook explores a bank marketing dataset to understand the factors influencing ad conversion rates. It uses visualizations and a decision tree model to identify key drivers of ad performance, providing insights into customer engagement.

**Source:** [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing) from the UCI Machine Learning Repository.

## Dataset

The dataset contains information about bank clients, including demographics, financial status, and interaction with marketing campaigns. The target variable is `converted`, indicating whether the client subscribed to a term deposit (1) or not (0).

**Key Features:**

* **Demographics:** age, job, marital status, education
* **Financial:** balance, housing loan, personal loan
* **Campaign:** contact type, number of contacts, month of contact
* **Other:** day of week, duration of last contact, previous campaign outcome


## Analysis

The notebook performs the following analysis:

* **Data Exploration:**  Calculates descriptive statistics and visualizes the data using box plots and violin plots to understand the distributions and relationships between variables.
* **Conversion Rate Calculation:** Calculates conversion rates by different features like number of contacts and job.
* **Data Preprocessing:** Encodes categorical variables (job, marital, education, etc.) using one-hot encoding.
* **Decision Tree Modeling:** Builds a decision tree model to predict conversion and visualizes the tree using Graphviz.
* **Feature Importance:**  Evaluates the importance of different features in the decision tree model.


## Key Findings

* **Balance:** Clients with higher bank balances tend to have higher conversion rates.
* **Campaign:**  The number of contacts influences conversion rates, with a sweet spot identified.
* **Job:**  Certain job categories show higher conversion rates than others.
* **Decision Tree:**  The decision tree model reveals the hierarchical importance of different features in predicting conversion.

## Dependencies

This project requires the following Python libraries:

* pandas
* matplotlib
* seaborn
* scikit-learn

You can install them using pip:

```bash
pip install pandas matplotlib seaborn scikit-learn graphviz
