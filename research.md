# Finance Tracker App - Research Report

**Date:** March 10, 2026  
**Purpose:** Personal finance app features analysis and improvement recommendations

---

## Current App Overview

Your finance tracker already includes:
- Net worth tracking (multi-currency support with BND/BTC)
- Asset management: Cash, Bank, BTC Ledger, Ledn Collateral
- Liabilities tracking: Ledn Loan
- Monthly income/expense tracking
- Transaction logging with categories
- Quick-add buttons for common transactions
- Real-time BTC price display
- Import/Export (JSON)
- Clean dark-themed mobile UI

---

## Industry Trends (2025-2026)

### What's Driving the Market
- **AI/ML Integration**: The biggest trend — apps now use AI for automatic categorization, predictive insights, and personalized financial advice
- **Cleaner Dashboards**: Industry-wide shift toward less clutter, more intuitive navigation
- **Automation**: Automatic transaction categorization, recurring payment detection, bill reminders
- **Holistic Wealth View**: Combining budgeting with net-worth tracking and investing
- **Real-time Sync**: Bank account aggregation via Plaid/MX APIs

### Top Features Users Expect
1. Automatic categorization (AI-powered)
2. Budget creation and tracking
3. Spending insights and trends
4. Goal setting (savings, debt payoff)
5. Bill reminders and due date tracking
6. Investment portfolio view
7. Credit score monitoring
8. Financial forecasting

---

## Recommended Improvements

### High Priority

**1. Automatic Transaction Categorization**
- AI learns from your manual categorizations
- Detects patterns (Netflix → "Entertainment", Salary → "Income")
- Reduces manual entry friction

**2. Budget Limits & Alerts**
- Set monthly limits per category
- Push notifications when approaching/exceeding limits
- Visual progress bars on spending

**3. Spending Insights & Trends**
- Weekly/monthly spending breakdowns (already have Chart.js)
- Category pie charts, trend lines
- "Your top spending categories this month" insights

**4. Recurring Transaction Detection**
- Auto-detect subscriptions (Netflix, gym, etc.)
- Flag recurring payments
- Option to mark as "recurring" for better forecasting

### Medium Priority

**5. Financial Goals**
- Savings goals (emergency fund, vacation, car)
- Debt payoff plans (avalanche/snowball methods)
- Progress visualization

**6. Bill Reminders**
- Due date tracking for loans, subscriptions
- Notification before due dates
- Calendar view of upcoming bills

**7. Cash Flow Forecasting**
- Predict next month's income/expenses based on history
- "Based on your patterns, you'll have $X surplus next month"

**8. Investment Portfolio Expansion**
- Beyond BTC: track stocks, crypto across exchanges
- Portfolio allocation pie chart
- Total returns calculation

### Lower Priority (Nice to Have)

**9. Credit Score Integration** (via Credit Karma / other APIs)
**10. PDF Report Generation** for taxes/record-keeping
**11. Cloud Backup** (iCloud, Google Drive)
**12. Multi-user / Shared Accounts** for couples
**13. Voice Input** for quick transaction entry

---

## Competitive Analysis

| App | Strength | Your Opportunity |
|-----|----------|-------------------|
| YNAB | Zero-based budgeting | Add budget envelopes feature |
| Empower | Holistic net-worth + investing | Expand investment tracking |
| PocketSmith | Forecasting | Add predictive cash flow |
| Quicken | Full financial picture | Add bill management |
| Piere | AI automation | Add smart categorization |

---

## Technical Considerations

- **Bank Sync**: Plaid API integration (requires backend, paid API)
- **AI Categorization**: Can start with rule-based, upgrade to ML
- **Data Storage**: LocalStorage → consider IndexedDB for larger datasets
- **Charts**: Already using Chart.js — leverage for trends/insights

---

## Suggested Next Steps

1. **Add budget limits per category** — quick win, high value
2. **Enhance charts** — spending trends, category breakdown
3. **Auto-categorization** — start with keyword matching, learn over time
4. **Goals tracking** — simple savings targets with progress

---

*This report provides direction for evolving your finance tracker from a basic expense logger into a comprehensive personal finance hub.*
