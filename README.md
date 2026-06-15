## 🔍 Methodology & Criteria

The pricing watchdog logic evaluates raw data feeds from official state government fuel monitoring databases according to the following rules:

1. **Price Anomaly Flagging**: Triggered by any single retail price spike of **$\ge 10.0\text{¢/L}$**.
2. **Episode Status Classification**:
   * **`GOUGE_CONFIRMED`**: A price spike that returns to or near baseline (or drops by at least $10.0\text{¢/L}$) within 48 hours.
   * **`SPIKE`**: An unresolved or sustained price spike.

## 🛠️ Automated Pipeline

These reports are automatically updated daily at **08:00 AM AEST** via a GitHub Action triggered from the [FullTank Fuel Monitor](https://www.fulltank.au) project.

---
## ⚖️ Legal Disclaimer & Limitation of Liability

**Please Read Carefully:**

1. **"As-Is" Provision**: All data, reports, and algorithmic analyses contained in this repository are provided on an "as-is" and "as-available" basis. No warranties of any kind—express, implied, or statutory—are made regarding the completeness, accuracy, reliability, timeliness, or usefulness of this information.
2. **Data Integrity & External Sources**: This dataset is parsed programmatically from public state-level government fuel price monitoring API feeds. We do not control, verify, or assume responsibility for errors, omissions, latency, or inaccuracies originating from these source feeds.
3. **Limitation of Liability**: In no event shall the repository owner, contributors, developers, or associated entities be liable for any claims, damages, liabilities, losses, or costs (including direct, indirect, incidental, special, punitive, or consequential damages, or loss of profits) arising out of or in connection with the access, use, or reliance on the data provided herein.
4. **No Professional or Legal Advice**: The contents of this repository are compiled for informational and consumer watchdog evaluation purposes only. They do not constitute financial, legal, business, or retail pricing advice. Users assume all risks associated with any decisions made based on this repository's contents.

