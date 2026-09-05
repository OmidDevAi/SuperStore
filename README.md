# SuperStore Sales Analysis & Machine Learning

## Project Overview

This project analyzes SuperStore sales data and uses machine learning models to predict order-level sales.

The project includes data cleaning, exploratory data analysis, business insights, data visualization, machine learning, model comparison, and interactive dashboards.

## Project Goals

The main goals of this project are:

* Understand sales and profit performance.
* Find important business patterns.
* Analyze sales by category, region, customer, and product.
* Study the relationship between discount and profit.
* Build machine learning models to predict order-level sales.
* Compare different machine learning algorithms.
* Select the best-performing model.

## Dataset

The dataset contains SuperStore order and sales information.

### Dataset Summary

| Metric           |         Value |
| ---------------- | ------------: |
| Rows             |         9,986 |
| Total Sales      | $2,295,509.57 |
| Total Profit     |   $286,013.82 |
| Loss-Making Rows |         1,870 |
| Unique Customers |           793 |

## Data Analysis

The project includes several steps of data analysis:

* Data cleaning and preprocessing
* Sales analysis
* Profit analysis
* Category analysis
* Sub-category analysis
* Regional analysis
* Customer analysis
* Product analysis
* Monthly sales analysis
* Discount and profit analysis
* Correlation analysis

## Business Insights

Some important findings from the analysis:

* **Technology** has the highest total sales.
* **Technology** also has the highest total profit.
* **West** has the highest total sales among the regions.
* A **50% discount** has the lowest average profit, with an average profit of **-$310.70**.
* **November 2022** was the strongest sales month, with sales of **$117,903.44**.

These results show that high discounts can have a negative effect on profitability and that sales performance can be different across categories and regions.

## Machine Learning

Five machine learning algorithms were trained and compared:

1. Linear Regression
2. Ridge Regression
3. Random Forest
4. Gradient Boosting
5. XGBoost

Tree-based models were tuned using **5-fold cross-validation**.

### Model Evaluation

The models were evaluated using:

* MAE — Mean Absolute Error
* MSE — Mean Squared Error
* RMSE — Root Mean Squared Error
* R² Score — Coefficient of Determination

## Model Comparison

| Model             |         MAE |        RMSE |   R² Score |
| ----------------- | ----------: | ----------: | ---------: |
| **XGBoost**       | **172.258** | **381.006** | **0.3555** |
| Gradient Boosting |     176.818 |     399.254 |     0.2923 |
| Random Forest     |     186.071 |     411.613 |     0.2478 |
| Ridge Regression  |     197.656 |     388.356 |     0.3304 |
| Linear Regression |     197.865 |     388.883 |     0.3286 |

### Best Model

**XGBoost** achieved the best overall test performance.

| Metric               |  Result |
| -------------------- | ------: |
| Cross-Validation MAE | 198.985 |
| Test MAE             | 172.258 |
| Test RMSE            | 381.006 |
| Test R²              |  0.3555 |

XGBoost was selected as the final model because it achieved the lowest test MAE and RMSE among the tested models and the highest R² score.

## Visualizations

The project contains visualizations for:

* Sales by category
* Sales by region
* Profit by category
* Profit by region
* Profit by sub-category
* Monthly sales trends
* Monthly profit trends
* Sales distribution
* Sales vs. profit
* Discount vs. profit
* Correlation heatmap
* Feature importance
* Actual vs. predicted sales
* Model comparison
* Top customers
* Top products
* Negative-profit products

The project also includes interactive HTML dashboards for exploring the results.

## Project Structure

```text
SuperStore/
│
├── data/
│   ├── raw/
│   │   └── superstore.csv
│   │
│   └── processed/
│       └── cleaned_superstore.csv
│
├── outputs/
│   ├── charts/
│   │   ├── actual_vs_predicted.png
│   │   ├── correlation_heatmap.png
│   │   ├── feature_importance.png
│   │   ├── model_comparison_mae.png
│   │   ├── model_comparison_r2.png
│   │   ├── model_comparison_rmse.png
│   │   └── ...
│   │
│   ├── models/
│   │   ├── best_model.joblib
│   │   └── preprocessor.joblib
│   │
│   └── reports/
│       ├── final_report.md
│       ├── model_comparison.csv
│       └── model_selection.csv
│
├── superstore_analysis (1).ipynb
├── Superstore-selected-columns.csv
├── .gitignore
└── README.md
```

## Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Joblib
* Plotly
* Jupyter Notebook

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/OmidDevAi/SuperStore.git
cd SuperStore
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 4. Install the required packages

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib plotly jupyter
```

### 5. Open the notebook

```bash
jupyter notebook
```

Then open:

```text
superstore_analysis (1).ipynb
```

## Limitations

This project predicts **order-level sales** and is not designed to forecast future monthly sales.

The model performance can also be improved by using additional features and more advanced feature engineering.

## Future Improvements

Possible future improvements include:

* Add time-based forecasting.
* Add customer-level features.
* Improve feature engineering.
* Test CatBoost and LightGBM.
* Build a simple prediction application.
* Improve the interactive dashboard.
* Use a time-based validation strategy for future forecasting.

## Key Takeaway

This project demonstrates a complete data analysis and machine learning workflow, from raw data cleaning to business insights and model evaluation.

The results show that **XGBoost performed best among the tested models**, while the analysis provides useful insights into SuperStore sales, profit, discounts, customers, products, and regions.

## Author

**Omid Rezapour**

GitHub: [OmidDevAi](https://github.com/OmidDevAi)
