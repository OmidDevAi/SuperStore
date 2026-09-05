# Final Project Report

## Project Goal
This project analyzes superstore sales data and builds machine learning models to predict order-level sales.

## Dataset Overview
- Rows: 9986
- Total sales: $2,295,509.57
- Total profit: $286,013.82
- Loss-making rows: 1870
- Unique customers: 793

## Business Insights
- Technology has the highest total sales.
- Technology has the highest total profit.
- West has the highest total sales among regions.
- The lowest average profit by discount level is at a discount of 50% with average profit of $-310.70.
- The strongest sales month is 2022-11 with sales of $117,903.44.

## Machine Learning
We trained Linear Regression, Ridge Regression, Random Forest, Gradient Boosting and XGBoost.
The models were compared using MAE, MSE, RMSE and R2.
Tree-based models were tuned with 5-fold cross-validation.

## Model Comparison
| Model | MAE | MSE | RMSE | R2 Score |
| --- | ---: | ---: | ---: | ---: |
| XGBoost | 172.258 | 145165.851 | 381.006 | 0.3555 |
| Gradient Boosting | 176.818 | 159404.065 | 399.254 | 0.2923 |
| Random Forest | 186.071 | 169425.172 | 411.613 | 0.2478 |
| Ridge Regression | 197.656 | 150820.363 | 388.356 | 0.3304 |
| Linear Regression | 197.865 | 151230.019 | 388.883 | 0.3286 |

## Model Selection
- Best model: **XGBoost**
- Cross-validation MAE: 198.985
- Test MAE: 172.258
- Test RMSE: 381.006
- Test R2: 0.3555

## Limitations
- The project predicts order-level sales, not future monthly sales.
- A time-based split can be useful for future forecasting.
- More customer and product features may improve the model.

## Future Improvements
- Add time-based forecasting.
- Add customer-level features.
- Test CatBoost and LightGBM.
- Build an interactive dashboard.
- Build a simple prediction application.
