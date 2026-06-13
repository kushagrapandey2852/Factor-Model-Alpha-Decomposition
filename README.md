<div align="center">

# 📊 Factor Model & Alpha Decomposition

### Fama-French Analytics • Performance Attribution • Factor Investing

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Statsmodels-Econometrics-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/Fama--French-5_Factor_Model-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/WRDS-Institutional_Data-orange?style=for-the-badge">
</p>

<p align="center">
  <b>Alpha Attribution</b> • <b>Factor Exposures</b> • <b>Rolling Regressions</b> • <b>Factor Momentum</b>
</p>

</div>

---

## Overview

Did a portfolio outperform because of manager skill?

Or because it was exposed to the right factors?

This project decomposes portfolio returns into systematic factor exposures and true alpha using the **Fama-French 5-Factor Model**.

The platform identifies where returns come from, measures changing factor sensitivities through time, and evaluates whether performance is driven by skill or risk-factor exposure.

---

## Factor Investing Framework

<div align="center">

```text
           Portfolio Returns
                    │
                    ▼

            Factor Model

                    │

      ┌─────────────┼─────────────┐

      ▼             ▼             ▼

 Systematic     Factor      Idiosyncratic
   Return      Exposure         Alpha

      │             │             │

      └─────────────┼─────────────┘
                    ▼

       Performance Attribution
```

</div>

---

## Fama-French 5-Factor Model

<div align="center">

```text
          Market Return
                 │
                 ▼

         Fama-French Model

                 │

     ┌───────────┼───────────┐

     ▼           ▼           ▼

   Size       Value    Profitability

                 │

                 ▼

           Investment

                 │

                 ▼

             Market
```

</div>

### Factors

| Factor | Description |
|----------|-------------|
| MKT-RF | Market Risk Premium |
| SMB | Small Minus Big |
| HML | High Minus Low |
| RMW | Robust Minus Weak |
| CMA | Conservative Minus Aggressive |

---

## Return Decomposition

<div align="center">

```text
 Portfolio Return

         │

         ▼

 ┌─────────────────┐
 │ Systematic Risk │
 └─────────────────┘

         +

 ┌─────────────────┐
 │     Alpha       │
 └─────────────────┘

         +

 ┌─────────────────┐
 │ Residual Noise  │
 └─────────────────┘
```

</div>

---

## Alpha Attribution Engine

<div align="center">

```text
 Historical Returns
          │
          ▼

 Factor Regression

          │

          ▼

 Estimated Betas

          │

          ▼

 Expected Return

          │

          ▼

 Alpha Estimate
```

</div>

### Objective

Determine whether performance arises from:

- Factor Exposures
- Manager Skill
- Random Noise

---

## Time-Series Regression

<div align="center">

```text
 Portfolio Returns

         │

         ▼

 OLS Regression

         │

         ▼

 Factor Betas

         │

         ▼

 Alpha Estimate
```

</div>

Measures sensitivity of a portfolio to each risk factor over time.

---

## Cross-Sectional Analysis

<div align="center">

```text
 Multiple Assets

          │

          ▼

 Factor Exposures

          │

          ▼

 Cross-Sectional Regression

          │

          ▼

 Factor Premia
```

</div>

Used to evaluate whether factor exposures explain return differences across securities.

---

## Rolling Factor Analysis

Factor exposures evolve through time.

<div align="center">

```text
 Window 1
    │
    ▼

 Window 2
    │
    ▼

 Window 3
    │
    ▼

 Window N

    │

    ▼

 Dynamic Betas
```

</div>

---

## Factor Momentum Engine

<div align="center">

```text
 Historical Factors

         │

         ▼

 Rolling Performance

         │

         ▼

 Factor Ranking

         │

         ▼

 Momentum Signals
```

</div>

Tracks persistence and cyclicality in factor performance.

---

## Performance Attribution Pipeline

<div align="center">

```text
 Portfolio

     │

     ▼

 Factor Exposure

     │

     ▼

 Return Contribution

     │

     ▼

 Alpha Decomposition

     │

     ▼

 Attribution Report
```

</div>

---

## System Architecture

<div align="center">

```text
┌─────────────────────────┐
│ WRDS Financial Data     │
└────────────┬────────────┘
             │
             ▼

┌─────────────────────────┐
│ Data Processing Layer   │
└────────────┬────────────┘
             │
             ▼

┌─────────────────────────┐
│ Factor Model Engine     │
├─────────────────────────┤
│ Fama-French Factors     │
│ OLS Regressions         │
│ Beta Estimation         │
│ Alpha Attribution       │
└────────────┬────────────┘
             │
             ▼

┌─────────────────────────┐
│ Rolling Analytics       │
└────────────┬────────────┘
             │
             ▼

┌─────────────────────────┐
│ Visualization Layer     │
└─────────────────────────┘
```

</div>

---

## Dashboard Components

| Module | Purpose |
|----------|---------|
| Factor Exposure Dashboard | Beta Analysis |
| Alpha Attribution | Return Decomposition |
| Regression Analytics | Model Statistics |
| Rolling Betas | Dynamic Exposure |
| Factor Momentum | Factor Trends |
| Portfolio Attribution | Performance Breakdown |
| Research Reports | Factor Insights |

---

## Quantitative Foundation

<div align="center">

```text
 Modern Asset Pricing

          │

          ▼

 Risk Factors

          │

          ▼

 Factor Models

          │

          ▼

 Performance Attribution

          │

          ▼

 Alpha Generation
```

</div>

---

## Example Attribution

```text
Portfolio Return = 14.2%

Market Factor      +6.1%
Size Factor        +1.8%
Value Factor       +1.2%
Profitability      +0.9%
Investment         +0.4%

Alpha              +3.8%
```

---

## Technology Stack

```text
Python
│
├── Pandas
├── Statsmodels
├── NumPy
├── Seaborn
└── WRDS Data
```

---

## Real-World Applications

### Asset Managers

- Portfolio Attribution
- Risk Exposure Monitoring
- Manager Evaluation

### Quantitative Analysts

- Factor Research
- Alpha Discovery
- Performance Analysis

### Equity Funds

- Style Drift Monitoring
- Portfolio Construction
- Factor Timing

---

## Skills Demonstrated

✅ Fama-French Models

✅ Asset Pricing

✅ Alpha Attribution

✅ Performance Decomposition

✅ Econometrics

✅ Cross-Sectional Regression

✅ Time-Series Analysis

✅ Factor Investing

✅ Quantitative Research

✅ Portfolio Analytics

---

## Repository Structure

```text
factor-model-alpha-decomposition/
│
├── data/
│
├── factor_models/
│   ├── fama_french.py
│   ├── regressions.py
│
├── attribution/
│   ├── alpha_engine.py
│
├── rolling_analysis/
│
├── momentum/
│
├── visualizations/
│
├── research/
│
└── README.md
```

---

<div align="center">

### 📊 Separate Skill From Exposure

*"Alpha explains performance. Factors explain everything else."*

</div>
