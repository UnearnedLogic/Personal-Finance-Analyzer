PROJECT: Personal Finance Transaction Analysis
CLIENT: Personal Finance Coaching Platform
ROLE: Data Analyst

ALL DATA HAVE BEEN DOWNLOADED FROM "https://www.kaggle.com/datasets/ramyapintchy/personal-finance-data"

OBJECTIVE:
Analyze transaction data to uncover spending patterns, financial risks, and provide strategic recommendations.

------------------------------------------------------------
PHASE 1 — DATA AUDIT & CLEANING
------------------------------------------------------------

1. Load the dataset and inspect structure:
   - Check shape (rows, columns)
   - Review data types
   - Preview first and last rows

2. Data Quality Checks:
   - Detect missing values in all columns
   - Identify duplicate rows
   - Check for negative or zero Amount values
   - Verify that "Type" column contains valid categories (Expense, Income, etc.)
   - Look for inconsistent category naming

3. Date Handling:
   - Convert Date column to datetime
   - Extract:
        • Year
        • Month
        • Month-Year
   - Check for invalid or out-of-range dates

4. Data Validation Rules:
   - Ensure Expenses have positive Amount
   - Check for extremely large outliers
   - Confirm there are no impossible transaction patterns

5. Deliverable:
   - Write a short summary of data issues found
   - Document all cleaning steps performed
   - State assumptions made during cleaning


------------------------------------------------------------
PHASE 2 — SPENDING STRUCTURE ANALYSIS
------------------------------------------------------------

OBJECTIVE:
Understand where money is going and visually communicate spending patterns.

------------------------------------------------------------
1. Total Spending Per Category
------------------------------------------------------------

Tasks:
- Filter only Expense transactions.
- Compute total spending per Category.
- Sort categories by total spending (descending).
- Calculate percentage contribution of each category.

Visualization:
- Create a bar chart showing total spending per category.
- X-axis: Category
- Y-axis: Total Spending
- Ensure categories are sorted from highest to lowest.
- Add title and axis labels.

Optional:
- Create a second bar chart showing % contribution per category.

Business Questions:
- What are the top 3 spending categories?
- Does one category dominate spending?
- Is spending diversified or concentrated?

------------------------------------------------------------
2. Frequency vs Average Transaction Analysis
------------------------------------------------------------

Tasks:
- Compute transaction count per category.
- Compute average transaction size per category.
- Combine into a summary table.

Visualization:
- Create a bar chart for transaction frequency per category.
- Create a separate bar chart for average transaction size.
- Compare visually:
    • High frequency categories
    • High average categories

Business Questions:
- Which categories are frequent small expenses?
- Which are rare but expensive?
- Which behavior pattern is riskier?

------------------------------------------------------------
3. Spending Distribution Analysis
------------------------------------------------------------

Tasks:
- Analyze overall distribution of Expense amounts.

Visualization:
- Plot histogram of transaction amounts.
- Observe distribution shape (normal? skewed?).
- Identify long right tail if present.

Business Questions:
- Are most transactions small?
- Are large transactions rare?
- Is spending right-skewed (typical financial pattern)?

------------------------------------------------------------
4. Category Volatility Analysis (Advanced)
------------------------------------------------------------

Tasks:
- Compute mean and standard deviation per category.
- Calculate coefficient of variation (std / mean).

Visualization:
- Bar chart of volatility (coefficient of variation) per category.
- Identify unstable categories.

Business Questions:
- Which categories have unpredictable spending?
- Are high-volatility categories also high-total categories?
- Where is financial risk concentrated?

------------------------------------------------------------
PHASE 3 — TIME-BASED TREND ANALYSIS
------------------------------------------------------------

Tasks:
- Compute monthly total spending.
- Compute monthly transaction count.
- Compute monthly average transaction.

Visualization:
- Line plot of monthly total spending.
- Line plot of monthly transaction count.
- Optional: Overlay income vs expense trends (separate plot).

Business Questions:
- Is spending increasing over time?
- Are there seasonal patterns?
- Are there spikes indicating instability?

------------------------------------------------------------
PHASE 4 — FINANCIAL RISK & ANOMALY DETECTION
------------------------------------------------------------

Tasks:
- Identify transactions above (mean + 2*std).
- Identify high-volatility months.
- Compute monthly risk score (based on volatility + large anomalies).

Visualization:
- Scatter plot showing outlier transactions.
- Line plot showing monthly volatility.
- Line plot showing monthly risk score.

Business Questions:
- When does financial instability peak?
- Are anomalies isolated or clustered?
- Is risk trending upward?

------------------------------------------------------------
PHASE 5 — STRATEGIC CONSULTING RECOMMENDATIONS
------------------------------------------------------------

Final deliverable must include:

- Tables supporting insights.
- Visual charts supporting conclusions.
- Written executive summary explaining:
    • Main spending drivers
    • Risk areas
    • Behavioral patterns
    • 3 strategic recommendations
    • Short-term and long-term actions

------------------------------------------------------------
FINAL NOTE:
Each visualization must include:
- Clear title
- Axis labels
- Logical sorting
- Business interpretation below chart
------------------------------------------------------------