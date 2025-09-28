Source: [YTM Analysis](https://github.com/katcohen/Fixed_income_Analysis/blob/main/YTM_analysis.ipynb)

Bond Valuation & Risk Analysis (5-Year, 4.5% Coupon)

---

## Executive Summary
- **Price:** **100.67** (per 100 face)  
- **Yield to Maturity:** **4.35%** (semiannual compounding)  
- **Premium:** Small, since **coupon (4.5%)** is slightly above market yield (4.35%).  
- **Key Risk Metrics:**  
  - **Duration:** ~4.44y  
  - **DV01:** ~4.5¢/bp  
  - **Convexity:** ~23.1  
  - **±10 bp yield change:** ≈ ±0.44% price move  
- **Portfolio View:** Moderate-risk, near-par bond well-suited for intermediate exposure.  
  - If rates **rise** → trim or hedge to reduce DV01.  
  - If rates **fall** → hold for coupon carry and convexity-driven upside.  

---

## Valuation
- **Price:** **100.67** per 100 face  
- **Yield to Maturity (YTM):** **4.35%** (semiannual compounding)  
- **Consistency check:** Backing out the yield from price gives **4.35%**, confirming pricing/yield functions align.  
- **Premium:** Slightly above par, since **coupon (4.5%) > yield (4.35%)**.  

**Decomposition of Price**  
- **PV of coupons:** 20.03  
- **PV of principal:** 80.64  
- **Share of value:** ~20% from coupons, ~80% from principal  

**Holding-Period Return (1-year, unchanged yields):** ≈ **4.35%**, almost entirely coupon-driven with only minor price drift (100.67 → ~100.55).  

---

## Risk Metrics (per 100 face, semiannual)

| Metric                | Value       |
|------------------------|-------------|
| **Macaulay duration**  | ~4.54 years |
| **Modified duration**  | ~4.44 years |
| **DV01**               | 0.0447 (~4.5¢ per bp) |
| **Convexity**          | ~23.1       |

**Interpretation:**  
- A **±10 bp yield move** implies ≈ **±0.44% price change** (before convexity).  

---

## Portfolio Implications
- **Risk profile:** Moderate, near-par bond suitable for anchoring intermediate (“belly”) exposure.  
- **DV01 scaling:** ~4.5¢ per bp can be used to size positions relative to a DV01 budget.  

**Positioning:**  
- **Bearish rates view:** Trim exposure or hedge (e.g., TY futures or pay-fixed IRS) to reduce DV01.  
- **Bullish rates view:** Hold position to capture coupon carry and convexity, without taking significant premium risk.  
