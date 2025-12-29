# JKSE-Forecasting-LSTM
Stock market forecasting for JKSE index using Stacked LSTM
# JKSE (IHSG) Index Forecasting: A Stacked LSTM & BI Analytics Approach

This repository demonstrates an end-to-end quantitative pipeline for predicting the **Jakarta Composite Index (JKSE)** closing prices. As a Mathematics student specializing in Financial Modeling, I developed this project to explore the synergy between Deep Learning architectures and Business Intelligence (BI) tools.

## 📌 Project Overview
Predicting stock market trends requires capturing complex, non-linear dependencies. This project utilizes a **Stacked LSTM (Long Short-Term Memory)** network, optimized for time-series forecasting. Beyond just modeling, the results are integrated into an interactive Tableau dashboard to provide actionable financial insights.

## 🛠️ Technical Methodology
The project follows a rigorous data science workflow:
- **Feature Engineering:** Implemented a 60-day sliding window to capture medium-term market cycles.
- **Model Architecture:** A Stacked LSTM configuration with Dropout layers (0.2) to ensure robust generalization and prevent overfitting.
- **Optimization:** Utilizing Adam optimizer and Mean Squared Error (MSE) loss function, with Early Stopping to preserve the best model weights.
- **BI Integration:** Model outputs are exported to a structured CSV format for advanced visualization in Tableau Desktop.

## 📊 Performance & Evaluation
The model's reliability is validated through historical backtesting on the test set:
- **Mean Absolute Error (MAE):** 57.50 IDR
- **Percentage Error:** ~0.68% (Given an index average of ~8,400 IDR)
- **Forecast Horizon:** 7-day out-of-sample recursive forecasting.

## 📈 Interactive Dashboard (Tableau)
The results are visualized in a multi-sheet Tableau dashboard, featuring:
1. **Trend & Forecast:** Comparative view of actual vs. predicted movements.
2. **Error Analysis (Residuals):** Visualizing model over/under-estimation periods.
3. **Price Distribution:** Analyzing market volatility density.

> **View the Interactive Dashboard:** [[INSERT YOUR TABLEAU PUBLIC LINK HERE](https://public.tableau.com/views/Book1_17669771240010/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)]
)]

## 📂 Repository Structure
- `LSTM/LSTM.ipynb`: Core analytical notebook (Python).
- `data/JKSE.csv`: Historical market dataset.
- `data/JKSE_LSTM_Results_Tableau.csv`: Consolidated data for BI tools.
