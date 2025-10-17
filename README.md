***

# 📈 Time Series Analysis: Monthly Anti-Diabetic Drug Sales in Australia (1991–2008)

Analyze and visualize time series data for monthly Australian anti-diabetic drug sales using Python, matplotlib, seaborn, and statsmodels.  
This mini-project demonstrates the basics of time series plotting and seasonal decomposition.

***

## 📖 Overview

This project analyzes the **monthly sales of anti-diabetic drugs in Australia** from July 1991 to June 2008 ([dataset source](https://raw.githubusercontent.com/selva86/datasets/master/a10.csv)).  
Key steps include:
- Loading and previewing the time series dataset.
- Visualizing trends using matplotlib and seaborn.
- Decomposing the time series into trend, seasonality, and residuals.

***

## 📝 Dataset

- **Source:** [a10.csv – Monthly anti-diabetic drug sales](https://raw.githubusercontent.com/selva86/datasets/master/a10.csv) (Selva Prabhakaran / public repository)
- **Columns:**
  - `date`: Month (YYYY-MM-DD)
  - `value`: Monthly sales (in $ million AUD)
- **Period:** 1991-07 to 2008-06 (204 months)

***

## ⚙️ Technologies Used

| Category      | Library         |
|---------------|----------------|
| Data Handling | pandas, numpy  |
| Plotting      | matplotlib, seaborn |
| Decomposition | statsmodels     |
| Environment   | Jupyter Notebook / Python Script |

***

## 🚀 How to Use

**Clone this repo or download the code. Then:**

1. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels
   ```

2. **Run the notebook/script:**  
   - `python a10_timeseries_analysis.py`  
   or open the notebook in Jupyter/Colab and run all cells.

***

## 🧑‍💻 Example Code Summary

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from statsmodels.tsa.seasonal import seasonal_decompose

df = pd.read_csv('https://raw.githubusercontent.com/selva86/datasets/master/a10.csv', parse_dates=['date'])
...
result = seasonal_decompose(df['value'], model='additive', period=12)
result.plot()
plt.show()
```

***

## 📊 Example Output

- **Line Plot:** Drug sales over time
- **Decomposition Plot:** Trend, seasonality, and residuals visualized

***

## 💡 Extensions & Ideas

- Forecasting future sales with ARIMA/SARIMA
- Anomaly detection in residuals
- Smoothing & noise reduction methods
- Interactive dashboard (Plotly, Dash, or Streamlit)

***

## 👩‍💻 Author

*Sarah S V*  
B.Tech – Artificial Intelligence and Data Science  
Rajalakshmi Institute of Technology, Chennai  
📧 *[sarahsv.codes@gmail.com]*
📧 *[https://www.linkedin.com/in/sarahsv3107/]*
***

## 📚 References

- [Original Dataset Source](https://raw.githubusercontent.com/selva86/datasets/master/a10.csv)
- [Seasonal decomposition - statsmodels docs](https://www.statsmodels.org/stable/generated/statsmodels.tsa.seasonal.seasonal_decompose.html)
- Python pandas, matplotlib, seaborn, statsmodels official docs

***

*For questions or suggestions, open an issue or reach out!*

***
