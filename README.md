# Trade Policy Shock: Pre- and Post-Tariff Import Patterns

## Overview
This project analyzes U.S. monthly import patterns around a defined tariff implementation date. The purpose is to organize and visualize observed import behavior before and after the cutoff using a consistent framework. The analysis is descriptive and does not attribute causality or evaluate policy effectiveness.

The workflow begins with a China-focused view and then applies the same segmentation and normalization approach to additional major U.S. trading partners (Vietnam, Mexico, and Canada) for comparison context.

---

## Key Questions
- How do monthly import patterns behave before and after the tariff implementation date?
- What post-tariff import pattern is observed when the view is restricted to the months after implementation?
- How can a consistent time-based framework be applied across multiple countries using the same metric and definitions?

---

## Data
- Monthly country-level U.S. import values
- Fields used in the notebook:
  - `CTY_NAME`
  - `month_date`
  - `import_value_usd` (or equivalent country-month import value)
- Country subset used for comparison:
  - China, Vietnam, Mexico, Canada

> Note: The notebook is written to be descriptive. Observed changes may reflect multiple factors beyond trade policy.

---

## Method Summary
1. **Time-based segmentation**
   - A single tariff implementation date is used to label records as **Pre-Tariff** or **Post-Tariff**.

2. **Normalization**
   - Import values are normalized within each country (z-score) to support pattern comparison over time without emphasizing scale differences.

3. **Visualization**
   - Line charts display normalized import behavior across time.
   - A focused post-tariff chart isolates China’s pattern after implementation.

---

## Project Files
- `Trade_Policy_Shocks_and_Business_Implications.ipynb` — main notebook
- `imports_monthly_by_country.csv` — monthly imports dataset (country-month level)

---

## How to Run (Step-by-Step)

### Option A: Run in Jupyter Notebook (local)
1. Open Anaconda Navigator
2. Launch **Jupyter Notebook**
3. Navigate to the folder containing:
   - `Trade_Policy_Shocks_and_Business_Implications.ipynb`
   - `imports_monthly_by_country.csv`
4. Open the notebook
5. In the top menu, click: **Kernel → Restart & Run All**
6. Confirm charts render without errors

### Option B: Run in VS Code (optional)
1. Open VS Code
2. Install the **Python** extension (Microsoft)
3. Open the project folder
4. Open the notebook file
5. Select your Python/conda environment when prompted
6. Click **Run All**

---

## Tools
- Python
- pandas
- matplotlib
- Jupyter Notebook

---
## Notes / Limitations
- This analysis is descriptive and does not infer causal impact.
- Imports may be influenced by macroeconomic conditions, seasonality, and supply chain dynamics.
- Additional datasets (e.g., port-level TEUs) can be explored as a separate extension to maintain project scope.

## Author
Kenya Moorer
