# Fear & Greed Index — Hyperliquid Trader Analysis

Analyzing how Bitcoin market sentiment relates to trader behavior and performance on Hyperliquid.

---

## Files

| File | Description |
|------|-------------|
| `fear_greed_index.csv` | Bitcoin Fear & Greed sentiment data |
| `historical_data.csv` | Hyperliquid historical trade data |
| `analysis.ipynb` | Main Jupyter notebook |

---

## Requirements

Python 3.8 or above is required.

Install dependencies:

```
pip install pandas numpy matplotlib seaborn jupyter
```

---

## Setup

1. Download or clone this repository
2. Place both CSV files in the same folder as the notebook
3. Run the following command in that folder:

```
jupyter notebook
```

4. Open `analysis.ipynb` in the browser

---

## How to Run

Open `analysis.ipynb` and run all cells from top to bottom.

| Cell | Description |
|------|-------------|
| Cell 1 | Import libraries |
| Cell 2 | Load datasets, check shape and missing values |
| Cell 3 | Clean timestamps, align by date |
| Cell 4 | Create daily metrics per trader |
| Cell 5 | PnL and win rate by sentiment |
| Cell 6 | Trade behavior by sentiment |
| Cell 7 | Trader segmentation |
| Cell 8 | Three insight charts |
| Cell 9 | Strategy recommendations |

---

## Output Charts

Running all cells will save these files in the same folder:

- `pnl_winrate_by_sentiment.png`
- `behavior_by_sentiment.png`
- `three_insights.png`

---

## Notes

- Both CSV files must be in the same directory as the notebook
- Only trades with a valid date and non-null Closed PnL are used
- Sentiment is grouped into three levels: Fear, Neutral, Greed
