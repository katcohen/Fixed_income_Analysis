Source: [DCF Analysis](https://github.com/katcohen/Fixed_income_Analysis/blob/main/DCF_Analysis.ipynb)

# Bond Valuation & Risk Snapshot

**Instrument:** 4-year bond, 10% annual coupon, redeemed at par (100)  
**Discount rate / yield to maturity:** 4.5%

---

## Valuation
- **Fair value (NPV):** **119.73**
- **Breakdown:**
  - Present value of coupons = **35.88**
  - Present value of principal = **83.86**
- **Takeaway:** At a required return of 4.5%, 119.73 is the “fair” price.
  - If market trades **below this** → undervalued (positive NPV).
  - If market trades **above this** → overvalued relative to hurdle rate.

---

## Interest-Rate Risk
- **Macaulay Duration:** 3.53 years  
- **Modified Duration:** 3.38 years  
- **DV01:** 0.0405 (≈ $4 per 100bp per 100 face)  
- **Convexity:** 15.5 years²  

**Implications:**  
- A ±10bp parallel move implies roughly **∓0.34–0.35% price change** (duration effect).  
- Convexity provides a slight cushion on rate increases and adds upside on rate declines.

---

## Investor Considerations
- **Carry vs. Price Risk:**  
  - Strong coupon income (10%), but trades at a premium, so price will pull toward par over time.  

- **Positioning:**  
  - If you expect **rates to rise**, consider trimming exposure or hedging using DV01 (reduce exposure by `bp × 0.0405`).  
  - If you expect **rates to fall**, maintaining exposure captures both carry and convexity benefits.  

- **Risk Budget:**  
  - With a 3.4-year duration, this bond carries moderate rate risk. It can be scaled up or down depending on the portfolio’s duration target.

---

## Key Figures
- Price: **119.73**  
- PV(coupons) / PV(principal): **35.9 / 83.9**  
- Macaulay / Modified duration: **3.53 / 3.38**  
- Convexity: **15.5**  
- Reprice at 5.0%: **117.73**  
- Reprice at 4.0%: **121.78**

---

### Summary
This bond offers attractive coupon income relative to its duration profile, but trades at a premium. Its moderate interest-rate sensitivity and convexity profile make it a solid carry position in stable or declining rate environments, while in a rising rate outlook, exposure should be actively managed using DV01 as a hedge tool.
