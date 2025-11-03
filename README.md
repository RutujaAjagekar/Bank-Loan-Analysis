# Bank Loan Analysis

## Goal

Analyzed 38,576 bank loans to understand portfolio health, identify trends, and find key insights about lending patterns and customer behavior. **86.2% of loans are performing well**, indicating a strong but monitored portfolio.

---

## Data

- **Size**: 38,576 loans across 50 US states
- **Period**: Full year 2021 (Jan 1 - Dec 12)
- **Source**: financial_loan_data_excel.xlsx

---

## Key Outputs

### 1. Portfolio Health
- **86.2%** of loans are performing (Fully Paid or Current)
- **13.8%** defaulted (Charged Off)
- **Total Funded**: $435.8M | **Total Collected**: $473.1M (108% recovery)
- **Average Interest Rate**: 12.05%
- **Insight**: Portfolio is mostly healthy but needs risk monitoring

### 2. Debt Consolidation Dominates
- **47.1%** of all loans are for debt consolidation (18,214 loans)
- Credit card payoff is second at 13%
- **Average Loan Size**: $11,296 | **Average DTI**: 13.3%
- **Insight**: Consolidation is the main product people want to reduce existing debt

### 3. Monthly Trends Are Steady
- Funding, collections, and applications stay consistent each month
- No major seasonal spikes
- **Loan Terms**: 73% are 36-month, 27% are 60-month
- **Insight**: Predictable business good for forecasting

### 4. Geographic Concentration
- States vary widely in lending volume
- Some states drive significantly more business
- **Insight**: Opportunity to expand in underperforming regions

### 5. Employment Stability Matters
- People with longer job history get more loans
- 23% of borrowers have 10+ years employment (most stable segment)
- **Insight**: Job stability correlates with loan approval/demand

### 6. Home Ownership Affects Repayment
- Homeowners vs. renters show different repayment patterns
- **Loan Grade Distribution**: B-grade dominates (30% of portfolio)
- **Insight**: Home ownership could be a risk factor in underwriting

---

## Visualizations (8 Charts)

1. Monthly funding trend
   ![Total_Funded_Amount_by_Month.png](./outputs/Total_Funded_Amount_by_Month.png)

2. Monthly collections trend
   ![Total_Payment_Amount_by_Month.png](./outputs/Total_Payment_Amount_by_Month.png)

3. Monthly applications trend
   ![Total_Loan_Applications_by_Month.png](./outputs/Total_Loan_Applications_by_Month.png)

4. States ranked by funded amount
   ![Total_Funded_Amount_by_State.png](./outputs/Total_Funded_Amount_by_State.png)

5. Loan term comparison by repayment
   ![Total_Amount_Recieved.png](./outputs/Total_Amount_Recieved.png)

6. Home ownership by repayment
   ![Home_Ownership_by_Total_Amount_Recieved.png](./outputs/Home_Ownership_by_Total_Amount_Recieved.png)

7. Total funded amount (summary)
   ![Total_Funded_Amount.png](./outputs/Total_Funded_Amount.png)

8. Total loan applications (summary)
   ![Total_Loan_Applications.png](./outputs/Total_Loan_Applications.png)

---

## How to Run

```bash
# Install dependencies
pip install -r requirements.txt

# Run analysis (Jupyter - recommended)
jupyter notebook Bank_Loan_Analysis.ipynb

# Or run Python script
python bank_loan_analysis.py
```

---

## Tech Stack

- Pandas (data wrangling)
- Matplotlib & Seaborn (charts)
- Plotly (interactive visualizations)
- Jupyter Notebook / Python

---

## Quick Stats

| Metric | Value |
|--------|-------|
| Total Funded | $435.8M |
| Total Collected | $473.1M |
| Loan Performance | 86.2% good, 13.8% default |
| Avg Interest Rate | 12.05% |
| Avg Loan Amount | $11,296 |
| Avg DTI | 13.3% |
| Avg Annual Income | $69,645 |
| Consolidation Loans | 47.1% of portfolio |
| 36-Month Terms | 73% | 60-Month Terms | 27% |
| Most Stable Borrowers | 23% have 10+ years employment |
| Top Loan Grade | B-grade (30% of portfolio) |

---

## Files

- `Bank_Loan_Analysis.ipynb` - Full analysis with code and visualizations
- `bank_loan_analysis.py` - Python script version
- `financial_loan_data_excel.xlsx` - Data file

## Google Colab
[Open in Google Colab](https://colab.research.google.com/drive/1TegQqE_QVqAdqqRulCtQ1DLoibpI202O?usp=sharing)
