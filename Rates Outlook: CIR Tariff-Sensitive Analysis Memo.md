Source: [CIR Tariff-Sensitive Continued Analysis](https://github.com/katcohen/Fixed_income_Analysis/blob/main/Rates%20Outlook%3A%20CIR%20tariff-sensitive_Cont.%20Analysis.ipynb)

# Rates Outlook — CIR (Tariff-Sensitive Scenarios)
**Date:** 2025-08-30  
**Analyst:** Katherine Cohen

## Key Metrics (Monte Carlo mean across 500 paths)
| Scenario | Avg rate | Ann vol | Time > 5.5% | Time < 3% | Terminal |
|---|---:|---:|---:|---:|---:|
| Baseline | 4.50% | 6.73% | 0.35% | 0.13% | 3.95% |
| Tariff escalation | 4.69% | 6.03% | 3.19% | 0.20% | 4.25% |
| De-escalation | 4.02% | 9.32% | 0.00% | 1.33% | 3.27% |

## Interpretation & Actions
- **Tariff escalation:** higher θ and σ → rates stay elevated longer with bigger swings. Keep **duration underweight** vs. benchmark (focus on 2–7y KRD), add **inflation protection**, and **trim HY/EM beta**; consider payer swaptions/CDX hedges.
- **Baseline:** still elevated but less volatile; keep duration light and curve risk modest (bear-flattening bias).
- **De-escalation:** faster normalization (higher k) — begin **adding duration** (belly→long end), upgrade credit quality, and scale into spreads on weakness.

*Method:* CIR, daily steps over 2y, 500 paths per scenario; metrics computed per path, then averaged. Feller holds for all parameter sets.
