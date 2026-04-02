# Case Study: Demand Forecasting and Inventory Optimization

## Problem

Retailers need enough inventory to avoid stockouts, but too much inventory increases holding cost and waste. The project goal was to forecast demand for a retail series and turn those predictions into practical inventory decisions.

## Dataset

- Retail sales data covering `2019-01-01` to `2023-12-31`
- About `4.57 million` rows
- `50` stores and `50` items
- Focus example: `store_1 / item_1`

## Workflow

1. Performed exploratory data analysis to understand seasonality and demand patterns.
2. Built forecasting baselines and machine learning models.
3. Compared forecasting quality using `MAE` and `RMSE`.
4. Translated forecast output into safety stock and reorder point decisions.

## Models Compared

- Baseline forecast
- Linear Regression
- Random Forest

## Results

| Metric | Result |
|---|---:|
| Baseline MAE | `11.73` |
| Linear Regression MAE | `7.33` |
| Random Forest MAE | `3.64` |
| Baseline RMSE | `15.71` |
| Random Forest RMSE | `4.52` |
| Safety Stock | `60.46` |
| Reorder Point | `386.58` |

## Business Value

This project is more than a forecasting exercise. It shows how model output can be translated into actions that an operations or supply chain team can use. On the sample series, the final model reduced MAE by about `69.0%` and RMSE by about `71.2%` versus the baseline, then converted the forecast into a safety stock and reorder point recommendation. That makes it stronger than a notebook that ends with model accuracy alone.

## What This Shows About Me

- I can work with large structured datasets.
- I can connect ML outputs to operations decisions.
- I can communicate project value in business terms, not only technical terms.

## Next Upgrade

- expand from one sample series to multiple store-item combinations
- compare forecasting approaches designed specifically for time series
- add cost-based decision logic instead of fixed service-level assumptions
