# 📊 Data Science Assignment: Trader Behavior vs Market Sentiment

Submission for the **Web3 Trading Team – Data Science Internship Assignment**. The project studies how aggregated trader activity (volume, trade count, realized PnL) relates to the Bitcoin Fear & Greed Index to uncover behavioral signals.

---

## 📁 Repository Structure
```
ds_Shubham_Kumar_Jha/
├── README.md
├── ds_report.pdf
├── notebook_1.ipynb                # Main Jupyter/Colab notebook (analysis & visuals)
├── notebooks/                      # Placeholder for additional notebooks
│   └── .gitkeep
├── needed/
│   ├── csv_files/                  # Input and processed data
│   │   ├── fear_greed_index.csv
│   │   ├── historical_data.csv
│   │   └── merged_daily_analysis.csv
│   └── outputs/                    # Generated figures
│       ├── profit_vs_sentiment.png
│       ├── trade_count_vs_sentiment.png
│       ├── volume_vs_sentiment.png
│       └── pnl_vs_sentiment_timeseries.png
```

---

## 🧠 Project Workflow
1. **Load & clean data** from historical transactions and the Fear & Greed Index.
2. **Aggregate metrics** by day (`total_volume`, `total_pnl`, `trade_count`).
3. **Merge sentiment** data with daily trader aggregates.
4. **Analyze & visualize** relationships using time series and correlation plots.

---

## 📈 Key Findings
- Higher profitability aligns with **Greed** phases and drops during **Extreme Fear**.
- Trader activity (volume and counts) spikes during **Greed** and **Extreme Greed**.
- Divergences between aggregate PnL and sentiment can hint at market tops or elevated risk.

---

## ▶️ Reproducing the Analysis

### Option 1: Google Colab (recommended)
- Open `notebook_1.ipynb` in Google Colab.
- Select `Runtime → Run all` to execute every cell.

### Option 2: Local Jupyter / JupyterLab
1. **Create and activate a virtual environment**
   ```
   python -m venv env
   # macOS/Linux
   source env/bin/activate
   # Windows
   env\Scripts\activate
   ```
2. **Install dependencies**
   ```
   pip install pandas matplotlib seaborn jupyterlab
   # or: pip install -r requirements.txt
   ```
3. **Launch Jupyter and run the notebook**
   ```
   jupyter lab
   ```
   Open `notebook_1.ipynb`, then `Run all` to reproduce plots and summaries.

---

## 📂 Datasets
| File | Description |
| --- | --- |
| `csv_files/fear_greed_index.csv` | Daily Bitcoin market sentiment values and categories |
| `csv_files/historical_data.csv` | Trader-level or market transaction history |
| `csv_files/merged_daily_analysis.csv` | Aggregated trader metrics merged with sentiment |

---

## 📊 Generated Outputs
| Plot | Description |
| --- | --- |
| `profit_vs_sentiment.png` | Correlation between daily PnL and sentiment levels |
| `trade_count_vs_sentiment.png` | Number of trades vs sentiment |
| `volume_vs_sentiment.png` | Total traded volume vs sentiment |
| `pnl_vs_sentiment_timeseries.png` | Time-series comparison of aggregate PnL and sentiment |

---

## 🛠️ Tools & Libraries
- Python 3
- pandas
- matplotlib, seaborn
- Jupyter Notebook / Google Colab

---

## 🧾 Notes
- `merged_daily_analysis.csv` includes `date`, `total_volume`, `total_pnl`, `trade_count`, `value` (Fear & Greed Index), and `sentiment`.
- All figures featured in the report are stored in `outputs/`.
- The notebook is self-contained and reproducible end-to-end.

---

## 🧑‍💻 Author
- **Name:** Shubham Kumar Jha
- **Role:** Data Science Intern – Web3 Trading Team (2025)

---