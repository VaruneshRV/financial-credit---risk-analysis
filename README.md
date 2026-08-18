# Corporate Credit Risk Analytics & Financial Health Assessment

## 📌 Problem Statement
Commercial banks require rigorous risk assessment frameworks to evaluate corporate credit applications. **Green Solutions Manufacturing Ltd.**, a sustainable drinkware manufacturer with over £50M in annual revenue, is seeking additional credit facilities to support expanding capital expenditures and sustainability initiatives. 

The primary challenge is to analyze the company's financial statements across FY 2022 and FY 2023, identify underlying balance sheet and cash flow risks (such as negative organic Free Cash Flow and working capital movements), and integrate macroeconomic industry trends to deliver an underwriting recommendation to the Credit Officer.

---

## ⚙️ Methods Used

### 1. Multiplier Normalization
* Standardized reporting metrics by mapping input data from thousands (£'K) to presentation outputs in millions (£'M) using a uniform scaling factor:
  Units Multiplier = 0.001

### 2. Quantitative Financial Statement Spreading
* **Profitability & Performance:** Evaluated core operating scale by adjusting operating earnings for depreciation and amortisation:
  * EBITDA = Operating Profit - (Depreciation & Amortisation Expense)
  * EBITDA Margin = (EBITDA / Total Revenue) * 100
* **Asset Tangibility & Capital Protection:** Measured loss-absorption cushions by isolating hard, recoverable assets from total assets:
  * Total Tangible Assets (TTA) = Total Assets - Intangible Assets - Goodwill
  * Tangible Net Worth (TNW) = TTA - Total Liabilities
* **Solvency, Liquidity, & Leverage Metrics:** Computed multiple turns and liquidity ratios to assess default risk:
  * Current Ratio = Current Assets / Current Liabilities
  * Gross Leverage = (Current Debt + Long-Term Debt) / EBITDA
  * Net Leverage = (Total Debt - Cash & Equivalents) / EBITDA
  * EBITDA Net Interest Cover = EBITDA / |Net Interest Expense|

### 3. Macroeconomic & Industry Trend Integration
* Synthesized market research data covering reusable water bottle market expansion (projected to reach US$ 11.5B by 2034) and reusable coffee cup growth (projected 5.8% CAGR to US$ 25B by 2031) to evaluate the borrower's market positioning.

---

## 🛠️ Tools Used
* **Microsoft Excel (Task 1 Financial Reporting Tool.xlsx):** Multi-tab financial model linking raw statements (I. Profit_Loss, I. Balance_Sheet, I. Cashflow) to dynamic report outputs (O. Report).
* **Python (pandas, openpyxl, python-docx):** Programmatic verification, ratio validation, and automated report compilation.
* **Financial Analysis & Credit Underwriting Frameworks:** Ratio spreading, working capital cycle tracking, liquidity stress-testing, and covenant design.

---

## 🔍 Key Findings

| Metric Category | Financial Parameter | FY 2022 | FY 2023 | Analysis & Credit Implications |
| :--- | :--- | :--- | :--- | :--- |
| **Performance** | **Total Revenue** | £31.54M | £53.82M | **+70.67% YoY growth** driven by strong consumer demand. |
| | **EBITDA** | £1.49M | £5.52M | **+269.68% growth** showing strong fixed overhead cost absorption. |
| | **Operating Margin** | 6.32% | 12.12% | **+580 bps expansion** reflecting operating efficiency gains. |
| **Position** | **Total Tangible Assets** | £51.63M | £61.67M | **>99% asset tangibility**, offering solid physical collateral backing. |
| | **Tangible Net Worth** | £23.21M | £31.13M | **+34.11% expansion** in equity capital cushion. |
| | **Cash & Cash Equivalents** | £19.38M | £17.58M | Maintained deep liquidity despite major capital investments. |
| **Solvency & Risk** | **EBITDA Interest Cover** | 2.08x | 17.53x | **+15.45x increase**, showing strong debt servicing capacity. |
| | **Gross Leverage** | 7.82x | 1.24x | **-6.58x reduction (84% decrease)** in gross debt risk. |
| | **Net Leverage** | -5.15x | -1.94x | **Net Cash Position** where cash reserves exceed total financial debt. |
| | **Current Ratio** | 1.88x | 1.38x | Tightened due to trade payables growth, but remains above benchmark limits. |

### Identified Credit Risks:
1. **Capital Expenditure Outflow:** Heavy capital expenditure (£8.01M in FY 2023) to fund property and equipment build-outs outpaced operating cash flows, resulting in negative organic Free Cash Flow.
2. **Trade Payable Dependence:** Accounts payable expanded to £10.03M as the client leveraged supplier terms to fund rapid inventory accumulation (£5.76M).
3. **Product & Innovation Risk:** High dependency on continuous R&D to meet evolving sustainability and net-zero targets introduces potential product obsolescence risk.

---

## 💡 Solutions & Recommendations

1. **Credit Facility Approval:** Approve the requested senior secured credit facility based on the borrower's **1.24x Gross Leverage**, **17.53x Interest Cover**, and sustainable industry tailwinds.
2. **Asset-Backed Structure:** Structure borrowings as Asset-Backed Lending (ABL) secured against the borrower’s **£61.67M in Total Tangible Assets**.
3. **Defensive Liquidity Covenant:** Institute a minimum liquidity covenant requiring the company to maintain at least **£10.00M in unencumbered cash and cash equivalents**.
4. **Payables & Inventory Surveillance:** Implement quarterly monitoring of accounts payable aging schedules and inventory turnover to manage supplier credit exposure and working capital strain.
