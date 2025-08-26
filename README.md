# Screen Time Analysis — Indian Kids

## Overview
This project investigates daily screen time among Indian children and identifies factors associated with exceeding the **2-hour guideline**.

**Methods used**
- Exploratory Data Analysis (EDA)
- Chi-square test + Cramér’s V (categorical association)
- **Welch’s t-test** *and* **Mann–Whitney U** (robustness check for group differences)
- Logistic regression with **odds ratios (ORs) + 95% CIs** and a forest plot

**Robustness note:** I intentionally ran both Welch’s t-test and Mann–Whitney U. Their conclusions were **consistent**, which increases confidence in the results.


## Conclusions
- **Urban vs. Rural:** Urban children showed higher average screen time.
- **Device type:** Device choice (e.g., tablet vs. phone) was associated with exceeding 2 hours.
- **Use mix:** A lower educational-to-recreational ratio (more recreational) was linked to higher odds of exceeding 2 hours.
- **Logistic model:** Key predictors remained significant after adjustment; ORs and CIs are reported in the notebook.
- **Consistency:** Both Welch and Mann–Whitney gave the same overall conclusions.


## Limitations
- Cross-sectional data (no cause effect).
- Self-reported measures (possible bias).
- Smallish sample size (estimates may be unstable).
- Potential unobserved factors (e.g., socio-economic factors, parental rules).

