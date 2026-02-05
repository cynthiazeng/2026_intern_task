# Summer 2026 Internship — Technical Assessment

Welcome! This assessment evaluates your analytical and coding skills through a realistic sample of the work we do. Pick one of the two tasks below, spend 3–4 hours max, and show us how you think.

If you enjoy this, you'll enjoy working with us.

**Please keep this assessment confidential.**

---

## Logistics Questions

Include your answers at the beginning of your report:

1. When can you start?
2. Do you need a US visa for a summer internship?
3. Interested in full-time after the internship?
4. Would you need visa sponsorship for full-time?
5. Expected compensation?
6. Anything else we should know?
7. Feedback on this assessment?

---

## Overview

You have two synthetic datasets from the same location:

| Dataset | Contents |
|---------|----------|
| `electricity_prices.csv` | Hourly futures & spot prices (1 year) |
| `temperature.csv` | Daily temperature (10 years) |

Pick **one** task. Doing both is optional.

---

## Data

### Electricity Prices

| Column | Description |
|--------|-------------|
| `datetime` | Timestamp |
| `futures_price` | Price known one day ahead ($/MWh) |
| `spot_price` | Actual settlement price ($/MWh) |

Trades are submitted one day ahead at the hourly futures price and settle at the hourly spot price.

### Temperature

| Column | Description |
|--------|-------------|
| `date` | Date (YYYY-MM-DD) |
| `temp_c` | Daily average temperature (°C) |

Weather drives electricity demand.

---

## Task 1: Trading Strategy

**Goal**: Design and backtest a trading strategy for next-day electricity.

**Requirements**:
- Build a strategy (spread, trend, mean-reversion, or your own idea)
- Backtest on out-of-sample data
- Report return, Sharpe ratio, and relevant metrics
- Discuss setup, assumptions, and limitations

**Hints** (optional):
- Weather affects prices
- Seasonality and intraday patterns exist
- You can ignore transaction costs

---

## Task 2: Weather Prediction

**Goal**: Analyze temperature patterns and predict cold winter days.

This one's intentionally open-ended — define your own target, pick your approach, and tell a compelling story.

**Suggested direction**:
1. **Explore**: Has temperature volatility changed over 10 years?
2. **Predict**: Build a model for cold winter days
   - Constraint: Only use data from 6+ months prior
   - Define your target (e.g., "days below 0°C in November", "cold spells lasting 5+ days")
3. **Evaluate**: How well does it work? What are the limitations?

We're curious to see what you build.

---

## Deliverables

### Report
- PDF or Markdown, **5 pages max** (appendix doesn't count)
- Include: logistics answers, executive summary, methodology, results, limitations
- **AI disclosure**: Feel free to use AI tools — just tell us how

### Code
- Jupyter notebook or Python scripts
- Runnable and commented
- Brief instructions if needed

### Appendix (optional)
- Extra visualizations or analysis

---

## Submission

Send your report and code to **cynthia@meteorologica.com**.

**Deadline**: Rolling basis — no fixed deadline, we review as submissions come in.

---

Good luck — we're looking forward to seeing your work.
