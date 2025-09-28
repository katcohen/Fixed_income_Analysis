{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "e216474e-c8ba-48e9-bdaa-a1f93dddfb14",
   "metadata": {},
   "source": [
    "# Bond Valuation & Risk Snapshot\n",
    "\n",
    "**Instrument:** 4-year bond, 10% annual coupon, redeemed at par (100)  \n",
    "**Discount rate / yield to maturity:** 4.5%\n",
    "\n",
    "---\n",
    "\n",
    "## Valuation\n",
    "- **Fair value (NPV):** **119.73**\n",
    "- **Breakdown:**\n",
    "  - Present value of coupons = **35.88**\n",
    "  - Present value of principal = **83.86**\n",
    "- **Takeaway:** At a required return of 4.5%, 119.73 is the “fair” price.\n",
    "  - If market trades **below this** → undervalued (positive NPV).\n",
    "  - If market trades **above this** → overvalued relative to hurdle rate.\n",
    "\n",
    "---\n",
    "\n",
    "## Interest-Rate Risk\n",
    "- **Macaulay Duration:** 3.53 years  \n",
    "- **Modified Duration:** 3.38 years  \n",
    "- **DV01:** 0.0405 (≈ $4 per 100bp per 100 face)  \n",
    "- **Convexity:** 15.5 years²  \n",
    "\n",
    "**Implications:**  \n",
    "- A ±10bp parallel move implies roughly **∓0.34–0.35% price change** (duration effect).  \n",
    "- Convexity provides a slight cushion on rate increases and adds upside on rate declines.\n",
    "\n",
    "---\n",
    "\n",
    "## Investor Considerations\n",
    "- **Carry vs. Price Risk:**  \n",
    "  - Strong coupon income (10%), but trades at a premium, so price will pull toward par over time.  \n",
    "\n",
    "- **Positioning:**  \n",
    "  - If you expect **rates to rise**, consider trimming exposure or hedging using DV01 (reduce exposure by `bp × 0.0405`).  \n",
    "  - If you expect **rates to fall**, maintaining exposure captures both carry and convexity benefits.  \n",
    "\n",
    "- **Risk Budget:**  \n",
    "  - With a 3.4-year duration, this bond carries moderate rate risk. It can be scaled up or down depending on the portfolio’s duration target.\n",
    "\n",
    "---\n",
    "\n",
    "## Key Figures\n",
    "- Price: **119.73**  \n",
    "- PV(coupons) / PV(principal): **35.9 / 83.9**  \n",
    "- Macaulay / Modified duration: **3.53 / 3.38**  \n",
    "- Convexity: **15.5**  \n",
    "- Reprice at 5.0%: **117.73**  \n",
    "- Reprice at 4.0%: **121.78**\n",
    "\n",
    "---\n",
    "\n",
    "### Summary\n",
    "This bond offers attractive coupon income relative to its duration profile, but trades at a premium. Its moderate interest-rate sensitivity and convexity profile make it a solid carry position in stable or declining rate environments, while in a rising rate outlook, exposure should be actively managed using DV01 as a hedge tool."
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.13.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
