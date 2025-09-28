# Credit Risk Snapshot — Merton (Structural) Model

**Setup (inputs from notebook)**  
- Asset value (**V₀**): \$25.0B  
- Face debt due at T (**D**): \$22.0B  
- Risk-free rate (**r**): 4.5%  
- Asset volatility (**σₐ**): 35%  
- Horizon (**T**): 1 year

---

## Headline Results (risk-neutral)
- **1-yr Probability of Default (PD): ~37.5%**  
- **Equity value (E₀): \$5.56B**  
- **Debt value (B₀): \$19.44B**  
- **Implied flat credit spread**: **~7.9% (~790 bps)**  
  - *Note:* your print line shows “7.86 bps” but that’s a **units bug** (see “Implementation note” below).

**Context:** A 1-yr PD near ~37% is in **distressed territory** (ballpark CCC/CC), indicating high refinancing risk and potential restructuring under this capital structure and volatility.

---

## Why the PD is high
- **Thin asset cushion:** Assets (\$25B) sit only ~13% above face debt (\$22B).  
- **High uncertainty:** 35% asset vol amplifies downside asset paths within 1 year.  
- **Short horizon:** With limited time, adverse shocks are less likely to “mean-revert” before maturity.

---

## Investor Takeaways
- **Capital structure risk:** Current leverage leaves little buffer; PD is very sensitive around D/V ≈ 0.9–1.0.  
- **Pricing cross-check:** With B₀ ≈ \$19.44B vs D = \$22B, the flat spread that discounts D to B₀ is **~7.9% (~790 bps)** over the risk-free rate — consistent with a stressed credit profile.  
- **Actionable levers:**
  - **De-lever / raise equity** or use asset sales to reduce D/V; PD should drop meaningfully.
  - **Term out / stagger maturities** to lower near-term default pressure.
  - **Strengthen liquidity** (cash, undrawn RCF) to extend runway.
  - **Covenants / collateral** to improve recovery profile and potentially reduce spread.

---

## Sensitivity (from your PD vs. leverage sketch)
- **PD rises steeply as D/V approaches 1.0.** Even modest de-leveraging from D/V ~0.88–0.90 can materially reduce PD.  
- Consider rerunning the notebook with **D = \$20B** (and/or **T = 2y**) to quantify sensitivity to capital structure and horizon.

---

## Implementation Note (units fix)
