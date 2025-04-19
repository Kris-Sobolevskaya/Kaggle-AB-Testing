#  A/B Testing: Ad Campaign Performance Analysis

##  Objective
This project evaluates the performance of two digital advertising strategies — **control** and **test** groups — to determine if the new approach (test group) significantly outperforms the current strategy in driving user engagement and conversions.

---

##  Methodology

### 1. Data Cleaning & Preparation
- Combined and labeled control and test group datasets.
- Renamed columns for consistency.
- Converted the `date` column to datetime format.
- Checked for and handled missing or inconsistent data.

### 2. Exploratory Data Analysis (EDA)
- Compared group-wise averages across:
  - `Website Clicks`
  - `Add to Cart`
  - `Purchase`
- Visualized trends using time-series plots and bar charts.
- Observed engagement patterns over time and between groups.

### 3. Statistical Testing
- Conducted **independent two-sample t-tests** and **Mann-Whitney U tests** for robustness.
- Hypotheses were tested for:
  - `Website Clicks`
  - `Add to Cart`
  - `Purchase`

---

##  Key Findings

| Metric           | Control Mean | Test Mean | Significance                    |
|------------------|--------------|-----------|---------------------------------|
| Website Clicks   | 78.4         | 85.2      |  Statistically significant     |
| Add to Cart      | 22.1         | 28.3      |  Statistically significant     |
| Purchase         | 6.7          | 7.1       |  Not significant               |

> **Insight:** The test group showed significantly better performance in driving **website clicks** and **add-to-cart actions**, but no statistically significant improvement in **purchases**. This implies stronger engagement, but potential friction in the final purchase step.

##  Recommendations
- Investigate conversion drop-off from cart to purchase.
- Explore segment-level performance by campaign or demographic.
- Consider A/B testing checkout page UX or incentives.
- If cost-effective, test group tactics could be scaled with refinement.

---

##  Files
- ``: Raw datasets.
- `KaggleABTesting.ipynb`: Main analysis script (EDA + hypothesis testing).
- `README.md`: Project overview and key results.

---

## 🛠️ Tech Stack
- Python (Pandas, SciPy, Seaborn, Matplotlib)
- Jupyter Notebook / Script
