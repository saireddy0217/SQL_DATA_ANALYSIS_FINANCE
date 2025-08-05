# 💰 sql data Analysis finance using SQL

This project demonstrates the creation and analysis of a personal or institutional investment portfolio using SQL. It tracks stock investments across various companies and computes key financial metrics such as Return on Investment (ROI), profit, and investment categories.

---

## 🚀 Features

- Track companies and their respective share quantities
- Add buy and current prices for stocks
- Automatically calculate:
  - Profit/Loss (Difference)
  - Return on Investment (ROI %)
  - Investment and ROI categories
- Summarize the portfolio performance
- Identify high-return stocks
- Categorize investments by quantity and profitability

---

## 🛠️ Tech Stack

- **Database:** MySQL / SQLite
- **Language:** SQL

---

## 🧾 Schema Overview

**Table: `revenue`**

| Column Name     | Data Type | Description                        |
|-----------------|-----------|------------------------------------|
| Material        | VARCHAR   | Company/Stock name                 |
| pi_amt          | INT       | Number of shares                   |
| BUY_PRICE       | INT       | Purchase price per share           |
| CURRENT_PRICE   | INT       | Current market price per share     |
| DIFF            | INT       | Price difference (Profit/Loss)     |
| ROI             | INT       | Return on Investment (%)           |

---

## 📊 Example Queries

### ✅ Total profit from all investments
```sql
SELECT SUM(DIFF) AS TOTAL_PROFIT FROM revenue;
