# 🛒 Costco Wholesale Corp. (COST) Valuation Portfolio

<p align="left">
  <img src="https://img.shields.io/badge/Methodology-DCF%20%7C%20Comps%20%7C%20Precedents-FF5733?style=for-the-badge" alt="Methodologies" />
  <img src="https://img.shields.io/badge/Sector-Consumer%20Defensive-007ACC?style=for-the-badge" alt="Sector" />
  <img src="https://img.shields.io/badge/Status-Active%20Build-brightgreen?style=for-the-badge&logo=github" alt="Status" />
</p>

---

## ⚡ Quick Pitch: Why Costco?
Most traditional retailers live and die by their product margins. **Costco plays a different game.** This portfolio breaks down how Costco effectively operates as a high-margin membership annuity service disguised as a giant warehouse club. 

---

## 🛠️ The Valuation Toolkit
Click on any of the core methodologies below to see how the sausage is made!

<details>
<summary><b>📈 1. The 5-Year DCF Model (Intrinsic Valuation)</b></summary>
<br>

*   **The File:** `Costco DCF.xlsx`
*   **The Engine:** Built on fully integrated statements (`IS`, `BS`, `CFS`) running a 5-year Unlevered Free Cash Flow forecast.
*   **The Brains:** Powered by a custom `2)WACC` calculator and a dynamic `DCF Fill in` sheet complete with growth rate sensitivity tables.
</details>

<details>
<summary><b>📊 2. Public Trading Comps (Relative Valuation)</b></summary>
<br>

*   **The File:** `Costco trading comp.xlsx`
*   **The Universe:** Side-by-side benchmarking against **Walmart (WMT)**, **Target (TGT)**, and **BJ's Wholesale Club (BJ)**.
*   **The Reality Check:** Mathematically tracks why the market happily pays a massive premium for Costco (handily showing off its LTM EV/EBITDA of ~39.1x and P/E of ~61.8x).
</details>

<details>
<summary><b>💼 3. Precedent Transactions (Takeout Valuation)</b></summary>
<br>

*   **The File:** `Costco Precedent Transactions.xlsx`
*   **The Deep Dive:** Historical M&A log analyzing actual retail corporate buyouts.
*   **The Data:** Evaluates transaction multiples from major sector plays by titans like **C&S Wholesale Grocers**, **SpartanNash**, and **Kroger**.
</details>

---

## 🧠 Key Insight Breakdown

```python
class CostcoValuationSuite:
    def __init__(self):
        self.ticker = "COST"
        self.wacc = 0.0864  # Calculated 8.64% WACC
        self.ltm_pe = 61.8   # Comps Multiple Baseline
        
    def execute_sanity_check(self):
        print(f"[RUNNING SYSTEM EVALUATION FOR {self.ticker}]")
        print(f" -> Core WACC Engine Discount Rate: {self.wacc * 100:.2f}%")
        print(f" -> Current Market Trailing P/E: {self.ltm_pe}x")
        
        # Testing valuation justification against structural moat
        membership_renewal = 0.90 
        if membership_renewal >= 0.90:
            return "🔥 SYSTEM STATUS: Premium valuation multiples mathematically supported by recurring annuity stream."

# Initialize and run the portfolio model checks
model_run = CostcoValuationSuite()
print(model_run.execute_sanity_check())
