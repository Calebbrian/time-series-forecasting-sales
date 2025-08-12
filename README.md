# Time Series Sales Forecasting

## Project Overview  
This project analyzes **5 years of monthly sales data (Jan 2018 – Dec 2022)** to forecast future sales using **ARIMA** and **Prophet** models. The goal is to provide accurate forecasts that help guide **inventory management, marketing strategies, staffing, and financial planning**.

---

## Key Insights
- **Seasonality**: Consistent year-end strength and mid-year dips.  
- **Trend**: Steady underlying growth over five years.  
- **Volatility**: Sales ranged from ~3,900 to 16,000 per month.

---

## Model Performance
| Model        | MAPE   | MAE   | RMSE   | Notes |
|--------------|--------|-------|--------|-------|
| **Prophet**  | ~6.4%  | 895   | 1,026  | Best at capturing seasonal peaks & dips |
| **ARIMA(1,1,1)** | ~10.2% | 1,322 | 1,594 | Flatter month-to-month profile |

**Recommendation**: Use Prophet as the main planning tool, with ARIMA as a benchmark.

---

## Forecast Highlights (Next Quarter Baseline)
| Month | Lower (-6.4%) | Base Forecast | Upper (+6.4%) | +10% Scenario |
|-------|--------------|--------------|--------------|---------------|
| Jan 2023 | 13,104 | 14,000 | 14,896 | 15,400 |
| Feb 2023 | 13,104 | 14,000 | 14,896 | 15,400 |
| Mar 2023 | 13,104 | 14,000 | 14,896 | 15,400 |

---

## Business Implications
- **Inventory**: Align procurement with forecasted demand and add safety stock for high-demand months.  
- **Marketing**: Increase campaigns before peak months; run targeted promotions in slower months.  
- **Operations**: Coordinate staffing and logistics to match demand patterns.  
- **Finance**: Use forecast ranges to set realistic revenue targets and budgets with clear risk buffers.  

---

## 🚀 Next Steps
1. Integrate Prophet forecasts into a live dashboard for tracking.
2. Update forecasts monthly with new sales data.
3. Enhance model accuracy by adding holiday, campaign, and pricing data as regressors.

---

## Repository Contents
- **`sales_data_5_years.xlsx`** – Historical sales data.  
- **`Time_Series_Forecasting_For_Sales.pdf`** – Original analysis report.  
- **`Time_Series_Sales_Forecast_Stakeholder_Report.docx`** – Stakeholder-friendly summary.  
- **`README.md`** – Project documentation.

---

## Tools & Libraries
- **Python** – Data cleaning, analysis, and modeling  
- **Pandas**, **NumPy** – Data processing  
- **Matplotlib**, **Seaborn** – Visualization  
- **Prophet**, **statsmodels** – Time series forecasting
