# Actuarial Claims Reserving & IBNR Estimation (Chain-Ladder / Development Method)

This repository contains an actuarial claims reserving model implemented in Excel (`Reserving.xlsx`). The project demonstrates the application of the **Chain-Ladder (Loss Development) Method** on historical claims triangles to estimate **Incurred But Not Reported (IBNR)** losses and ultimate claims liabilities for general insurance portfolios.

---

## Project Overview & Objectives

In general insurance actuarial practice, estimating unpaid claim liabilities (outstanding claim reserves and IBNR) is critical for maintaining solvency and accurate financial reporting.

### Key Objectives & Analysis:
1. **Claims Triangle Construction:**
   - **Reported Claims Triangle:** Conversion of incremental reported losses into cumulative loss development triangles (Accident Years 1998–2007 across 12 to 120 months of development).
   - **Paid Claims Triangle:** Analysis of cumulative paid loss developments.
2. **Loss Development Factors (LDF) & Cumulative Factors (CDF):**
   - Calculation of age-to-age development factors ($\text{LDF}$) to project future claims growth.
   - Derivation of Cumulative Development Factors ($\text{CDF}$) to project ultimate losses.
3. **Ultimate Claims Projection:**
   - Estimation of ultimate losses using both **Reported Claims** and **Paid Claims** development methods.
4. **Reserve & IBNR Quantification:**
   - Separation of total reserve liabilities into **Case Outstanding (Case O/S)** reserves and **IBNR** estimates.
   - Comparative evaluation between reported-based and paid-based loss development results.

---

## Key Results Summary (As of 31/12/2007)

| Metric | Reported Claims Method | Paid Claims Method |
| :--- | :--- | :--- |
| **Cumulative Claims Evaluated** | RM 543,481,587 | RM 498,050,368 |
| **Projected Ultimate Claims** | RM 568,932,870 | RM 574,028,495 |
| **Case Reserves (Case O/S)** | RM 45,431,219 | RM 45,431,219 |
| **Estimated IBNR Reserve** | **RM 25,451,283** | **RM 30,546,908** |
| **Total Unpaid Claim Liability** | **RM 70,882,502** | **RM 75,978,127** |

---

## Workbook Structure (`Reserving.xlsx`)

* **`Raw Data`**: Contains initial incremental reported claims and cumulative paid claims data by accident year (1998–2007).
* **`Reported Claims`**: Cumulative reported claims triangle and age-to-age loss development factor calculations.
* **`Paid Claims`**: Cumulative paid claims triangle and paid age-to-age development analysis.
* **`Projection`**: Computation of CDFs and projected ultimate claims across all accident years.
* **`Development`**: Final reserve breakdown quantifying Case Outstanding, IBNR, and Total Unpaid Liabilities.

---

## Technical Methodologies Used
* **Chain-Ladder / Loss Development Method (LDM)**
* **Cumulative Development Factor ($\text{CDF}$) Link-Ratio Analysis**
* **IBNR Calculation:** $\text{IBNR} = \text{Projected Ultimate Claims} - \text{Latest Cumulative Reported Claims}$
* **Total Unpaid Liability:** $\text{Total Reserve} = \text{Case O/S} + \text{IBNR}$
