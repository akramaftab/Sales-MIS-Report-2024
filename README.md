# Sales Performance MIS Dashboard — Q1 2024

## Project Overview

This project builds a fully operational Sales MIS reporting system covering **120 transactions across 4 regions, 5 product lines, and 10 sales reps** over Q1 2024 (January–March). The system consolidates raw sales data into automated dashboards, pivot-based performance summaries, and a validated data entry layer — replacing fragmented manual reporting with a single source of truth.

The goal: give sales leadership real-time visibility into target achievement, rep-level performance gaps, product return risks, and regional variance — so decisions are driven by data, not gut feel.

> **Overall Q1 Achievement: 100.17%** | Total Net Sales: ₹2,77,989 | Returns Contained at 4.04%

---

## Repository Structure

```
Sales_MIS_Report_2024.xlsx
├── Raw_Data              → 120 transaction records (Jan–Mar 2024)
├── Monthly_Summary       → Region-wise monthly target vs actual with RAG status
├── Pivot_Analysis        → Salesperson & product performance rankings
├── Dashboard             → Q1 KPI scorecard with regional & monthly breakdowns
└── Data_Validation_Sheet → Controlled data entry with dropdown validations
```

---

## Process

**Data Collection & Structuring:**
Imported 120 sales records covering transaction date, region, product category, salesperson, target, actual sales, returns, and net sales across Q1 2024.

**MIS Dashboard Design:**
Built a multi-sheet Excel MIS system with KPI scorecards, RAG (Red-Amber-Green) status flags, pivot-based rep/product rankings, and a controlled data entry sheet with dropdown validations to prevent input errors.

**Performance Analysis:**
Analyzed regional variance, salesperson productivity gaps, product return rates, and monthly trends to surface actionable insights for sales leadership review.

**Reporting Logic:**
Structured the workbook for weekly refresh — new raw data flows into the data entry sheet, all summaries and dashboards update automatically via linked formulas and pivot tables.

---

## Key Findings

- **Q1 target achieved at 100.17%** (₹2,89,684 actual vs ₹2,89,189 target) — on the surface, clean. Under the hood, significant regional and rep-level variance.
- **West region overperformed at 107.38%** while North underperformed at **94.98%** — a 12.4 percentage point gap demanding targeted intervention.
- **Top rep (Rohit Patel) outperformed bottom rep (Vikram Rao) by 3.4x** in absolute sales — indicating an uneven workload distribution and potential for rep-level coaching.
- **February was the strongest month at 106.63% achievement** (₹1,10,661 actual); March dipped to 96.45% — suggesting an end-of-quarter slowdown worth flagging.
- **Product B and Product C led with 103.66% and 102.66% achievement** respectively; Product E lagged at 96.19% with ₹2,378 in returns.
- **West region carried the highest return rate at 4.71%** vs North at 3.53% — potential quality or fulfilment issue concentrated in one zone.
- **3 of 10 reps missed target** (Arun Kumar 98.65%, Neha Gupta 96.08%, Priya Singh 94.28%, Vikram Rao 93.18%) — bottom quartile averaging 95.5% vs top quartile at 105.7%.
- **South region turned around mid-quarter** — underperformed in January (90.25%) but recovered to 101.61% overall by March.

---

## Business Recommendations

- **Address the North region gap immediately:** At 94.98% achievement and ₹3,694 adverse variance, North needs a pipeline review and sales activity audit before Q2 planning.
- **Investigate the March slowdown:** February's momentum didn't carry into March (96.45%). Identifying whether this is a demand, dispatch, or rep-activity issue prevents a repeat in Q2.
- **Build a rep performance playbook from top performers:** Rohit Patel, Rahul Verma, and Sunita Joshi consistently exceed targets. Document their activity patterns and use as a benchmark for coaching the bottom four.
- **Review Product E's positioning:** At 96.19% achievement and a 3.56% return rate, Product E shows both a demand and quality signal — needs SKU-level review with the product/supply chain team.
- **Implement return rate thresholds by region:** West's 4.71% return rate should trigger an alert. Recommend setting a 4% ceiling as a KPI flag for logistics/quality escalation.
- **Automate RAG escalation:** Monthly Summary's Amber/Green status flags should trigger weekly manager notifications — removing the need for manual report chasing.
- **Expand to Q2–Q4 for full-year trend analysis:** Quarterly data alone limits pattern detection. A rolling 12-month MIS view would expose seasonality, rep burnout cycles, and product lifecycle signals.

---

## Tools & Techniques

| Tool / Feature | Application |
|---|---|
| Microsoft Excel | Multi-sheet MIS workbook, KPI dashboard |
| Pivot Tables | Salesperson & product performance ranking |
| Data Validation | Dropdown-controlled data entry to prevent input errors |
| Conditional Formatting | RAG status flags (Red/Amber/Green) for instant visibility |
| Linked Formulas | Auto-updating summaries on data refresh |
| Python (pandas) | Data inspection, statistical analysis, finding extraction |

---

## Dashboard Preview

> *(Screenshot of Dashboard sheet — add `Dashboard_Screenshot.png` here)*

```
📊 SALES MIS DASHBOARD — Q1 2024
─────────────────────────────────────────────────────
Total Target   Total Actual   Achievement %   Top Region
₹2,89,189      ₹2,89,684         100.2%          West
─────────────────────────────────────────────────────
Region    Target     Actual    Achievement
North     ₹92,761    ₹88,100      94.98% 🟡
South     ₹70,590    ₹71,726     101.61% 🟢
East      ₹57,471    ₹56,443      98.21% 🟡
West      ₹68,367    ₹73,415     107.38% 🟢
```

---

## Related Projects

- [Hotel Booking Cancellations Analysis](https://github.com/akramaftab/Python_Power_BI_-Hotel_analysis_project) — Python + Power BI | 119K bookings | Cancellation risk modeling
- [Pizza Sales Dashboard](#) — SQL + Power BI | Revenue & order trend analysis
- [Employee Attendance Tracker](#) — Excel + openpyxl automation

---

*Built as part of an MIS/Data Analytics portfolio targeting business analyst and MIS executive roles in manufacturing, FMCG, and e-commerce sectors.*
