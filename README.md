# Market Response Modeling

**University project** analyzing the effectiveness of different marketing communication channels on customer acquisition for a telecom company using **multiple linear regression**.

## Problem

Analyze **118 weeks** of telecom marketing data to determine which channels drive new customer acquisition most effectively:

- **Traditional advertising** (TV, radio, print, OOH)
- **Facebook impressions** (likes, comments, shares)
- **Twitter sentiment** (volume and valence)
- **Control variables** (holidays, media events, promotions)

**Objective**: Quantify channel effectiveness and provide actionable recommendations for marketing budget allocation.

## Approach

1. **Data Classification**: Variables categorized using the market response framework (marketing actions → observed output).
2. **Model Specification**: Multiple linear regression with **lagged effects** (1-week delay) to account for carryover effects.
3. **Model Diagnostics**: Tested assumptions, statistical significance, model fit (R², adjusted R², F-statistic).
4. **Channel Comparison**: Coefficient analysis and p-values to rank channel effectiveness.

## Model Results
Model Performance:

R²: 0.4277 (42.77% variance explained)

Adjusted R²: 0.3857

F-statistic: 10.18 (p < 1.565e-10)

Channel Effectiveness (ranked):

Twitter Valence: +1% valence → ~1 new customer (p < 0.05)

Traditional Advertising: €1000 spend → ~1 new customer (p = 1.43e-5)

Twitter Volume: Negative effect (-0.282 customers per message increase)

Facebook Impressions: Not significant (p = 0.494)

## Key Findings

- **Twitter sentiment (valence)** is the **most effective** acquisition driver
- **Traditional advertising** remains valuable (~1 customer per €1000)
- **Facebook impressions** show no statistically significant impact
- **Dynamic effects** (lagged variables) improve model accuracy

## Business Recommendations

1. **Prioritize Twitter sentiment management** over raw volume
2. **Maintain traditional advertising** as secondary channel
3. **Reallocate Facebook budget** to higher-ROI channels
4. **Consider lagged effects** in future campaign planning
