# RegimeLens MVP Final Submission

RegimeLens is an explainable AI prototype for **single-asset market regime detection**. This MVP uses historical Apple (AAPL) price data, basic technical indicators, and KMeans clustering to identify interpretable market regimes.

## Included files
- `RegimeLens_MVP.ipynb` — runnable notebook for the end-to-end demo
- `dataset.csv` — cleaned historical dataset used by the notebook
- `regime_results.csv` — final row-level output with detected regimes
- `regime_summary.csv` — cluster summary and explanations
- `RegimeLens_Final_Presentation.pptx` — final presentation deck
- `requirements.txt` — Python dependencies
- `outputs/` — exported charts used in the presentation

## Data source
- Asset: **AAPL**
- Source file: Plotly public sample dataset
- URL: https://raw.githubusercontent.com/plotly/datasets/master/finance-charts-apple.csv

## MVP workflow
1. Load dataset
2. Clean and prepare historical price data
3. Generate technical indicators: return, MA20, RSI14, volatility
4. Standardize features and run KMeans clustering (`k=3`)
5. Name the clusters as interpretable market regimes
6. Visualize regimes on the price chart
7. Export results to CSV

## How to run
```bash
pip install -r requirements.txt
jupyter notebook RegimeLens_MVP.ipynb
```
