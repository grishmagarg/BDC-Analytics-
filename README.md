# ⬡ Private Credit BDC Analytics Suite

> **A zero-install, browser-based analytics platform designed to analyze SEC Schedule of Investments (SOI) filings across private credit Business Development Companies (BDCs).**  
> Uncover shared borrowers, evaluate portfolio concentration, track valuation marks across managers, and detect emerging credit stress.

[![Live Application](https://img.shields.io/badge/Live%20Demo-grishmagarg.github.io%2Fbdc--credit--analytics-blue?style=for-the-badge&logo=github)](https://grishmagarg.github.io/bdc-credit-analytics)
[![Privacy First](https://img.shields.io/badge/Privacy-100%25%20Client--Side-green?style=for-the-badge)](https://grishmagarg.github.io/bdc-credit-analytics)
[![Zero Install](https://img.shields.io/badge/Run%20in%20Browser-Zero%20Install-orange?style=for-the-badge)](https://grishmagarg.github.io/bdc-credit-analytics)

---

### 🔗 **Live Application:** [grishmagarg.github.io/bdc-credit-analytics](https://grishmagarg.github.io/bdc-credit-analytics)

*(Runs 100% locally in your web browser — zero backend, no installations, no accounts required, and no data uploaded to external servers.)*

---

## 🚀 How to Run It (In 3 Clicks)

You do not need to download any files or know how to code to see this tool in action:

1. **Open the App**  
   Click the [Live Application Link](https://grishmagarg.github.io/bdc-credit-analytics).
2. **Fetch Data**  
   Click the **⚡ Load Sample Data** button at the top of the page. This automatically loads two quarters of real-world sample data (~11,000+ loan records across 10 top private credit funds) into the tool.
3. **Analyze**  
   Click the blue **⊙ Scan Files & Detect Funds** button.

🎉 **Done!** The tool is now fully populated. You can navigate through the different views using the tabs across the top.

---

## 🧭 What Does Each Tab Show?

### 1. 🔍 Overlap Analysis *(Shared Investments)*
- **What it does:** Select up to **five different investment funds** to see exactly which companies they all lent money to.
- **Why it matters:** If you invest in multiple funds hoping to diversify your risk, this view reveals if those funds are actually just lending money to the exact same businesses.
- **Visual Signals:** Spot the health of shared loans through color-coded numbers:
  - 🟢 **Green:** Indicates a healthy loan priced near par.
  - 🔴 **Red (under 90%):** Warns that the loan is stressed and the borrower might be struggling to pay it back.

---

### 2. 📊 Overlap Matrices *(The Big Picture Heatmap)*
- **What it does:** Generates a color-coded grid (heatmap) comparing every fund against every other fund.
- **Why it matters:** Gives you an instant, birds-eye view of how similar the portfolios are.
- **Visual Signals:** The darker or warmer the color, the higher the overlap. For example, a dark red box between two funds means their portfolios are highly identical and exposed to the exact same risks.

---

### 3. 🛡️ Level 3 Debt *(Risk Radar)*
- **What it does:** Acts as an automated stress test measuring the percentage of a fund's total money tied up in loans that are currently losing value.
- **Valuation Tiers:** Tracks loans valued at less than **70%**, **80%**, or **90%** of their original cost.
- **Why it matters:** Clearly highlights which fund managers are holding the highest concentration of risky or deteriorating assets relative to their total fund size.

---

### 4. 📈 Pricing Trend *(Health Over Time)*
- **What it does:** Tracks how the value of shared loans changes from one financial quarter to the next to highlight momentum.
- **Why it matters:** A loan might look fine today, but this tab automatically flags if its value has been rapidly dropping over the last six months, helping you spot deteriorating assets before they default.

---

### 5. 📉 Valuation Chart *(The "Difference of Opinion" Chart)*
- **What it does:** A visual line chart for any single company comparing how different funds value the exact same loan over time.
- **Why it matters:** Because private market managers estimate the value of their own loans, this chart exposes when one manager thinks a company is doing great (valuing the loan at 100%) while another manager thinks the exact same company is failing (valuing it at 80%).

---

## 🛡️ Privacy & Technical Architecture

- **100% Client-Side Computing:** All parsing and analytics run locally in memory via SheetJS and Chart.js.
- **Zero Data Ingestion:** Your filings never leave your machine or get sent to third-party servers.
- **SEC Filing Ready:** Designed for Schedule of Investments (SOI) standardized reporting.
