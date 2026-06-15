## 🔍 Methodology & Criteria

The pricing watchdog logic evaluates raw data feeds from official state government fuel monitoring databases according to the following rules:

1. **Price Anomaly Flagging**: Triggered by any single retail price spike of **$\ge 10.0\text{¢/L}$**.
2. **Episode Status Classification**:
   * **`GOUGE_CONFIRMED`**: A price spike that returns to or near baseline (or drops by at least $10.0\text{¢/L}$) within 48 hours.
   * **`SPIKE`**: An unresolved or sustained price spike.

## 🛠️ Automated Pipeline

These reports are automatically updated daily at **08:00 AM AEST** via a GitHub Action triggered from the [FullTank Fuel Monitor](https://www.fulltank.au) project.

---
*Disclaimer: The data compiled in these reports is retrieved directly from public state-level fuel databases. Analysis is performed algorithmmatically.*
