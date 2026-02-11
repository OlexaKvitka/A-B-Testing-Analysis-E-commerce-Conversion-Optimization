# A-B-Testing-Analysis-E-commerce-Conversion-Optimization

## Project Purpose:
Analyze the results of 4 A/B tests using statistical methods (z-test) in Python to determine which variations significantly improve conversion metrics and create a visualization. which will represent it

## Methodology
- **Statistical Test:** Two-proportion z-test
- **Significance Level:** α = 0.05
- **Metrics:** Begin Checkout Rate, Add Payment Rate, Add Shipping Info Rate, New Account Rate

## Deliverables:
1. Python statistical analysis in Google Colab Notebook: https://colab.research.google.com/drive/1At34zP646Xkgx3EasOvtfQB2H3FMfcPI?usp=sharing
2. CSV file with result extract: https://drive.google.com/file/d/1bYT0VibyKs7ja1Gif30sg5XK2tG1wZAq/view?usp=sharing
3. Tableau dashboard: https://public.tableau.com/views/ABTest_17638526161470/ABtest?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Project Structure
- **STEP 1:** Data Collection and Overview
- **STEP 2:** Data Transformation (Pivot Tables)
- **STEP 3:** Conversion Rate Calculation
- **STEP 4:** Statistical Significance Testing
- **STEP 5:** Visualization & Results
- **STEP 6:** Conclusions & Recommendations
  
## Conclusions & Recommendations
A/B Testing Analysis: Conversion Optimization Consequences
Overview
Analyzed 4 website variations across estimated 45K-105K sessions per group using two-proportion z-tests (α=0.05).

Tests evaluated impact on 4 conversion funnel metrics: payment submission, shipping information, checkout initiation, and account creation.

Result and recommendation by Test
Test 1: Statistically Significant Positive Results

New Account Rate: 8.43% -> 8.15% (-3.4%, p=0.123)
Begin Checkout Rate: 8.34% -> 8.90% (+6.7%, p=0.003)
Add Shipping Rate: 6.69% -> 7.13% (+6.6%, p=0.002)
Add Payment Rate: 4.38% -> 4.93% (+12.5%, p< 0.001)
Three out of four metrics show statistically significant improvement. The payment rate lift from 4.38% to 4.93% is hight potential revenue driver.Only account creation declined slightly, though not significantly.

Recommendation: implement as impact maker with measurable business value.

Test 2: Inconclusive results with no statistical significance

All metrics show slight positive trends (+1.2% to +3.6%).
No results reach statistical significance (p-values range 0.215-0.556).
Possible reasons: insufficient sample size, minimal design changes, or true null effect.

Recommendation:

Option A: Run extended test with larger sample size
Option B: Redesign variation with more substantial changes
Option C: Deprioritize in favor of more impactful tests
Test 3: Significant Negative Impact on Checkout

Begin Checkout Rate: 13.61% -> 13.15% (-3.4%, p=0.012)
Other metrics show non-significant changes
The checkout decline is statistically significant and commercially meaningful
Higher baseline rates (13.61% vs 8.34% in Test 1) suggest a different user segment or test conditions
Variation likely introduced friction at the checkout entry point.
Recommendation: don't implement. Analyze user behavior to understand friction points.

Test 4: Multiple Significant Declines

Begin Checkout Rate: 11.95% -> 11.67% (-2.4%, p=0.046)
New Account Rate: 8.55% -> 8.26% (-3.4%, p=0.018)
Add Payment Rate: 3.55% -> 3.42% (-3.5%, p=0.116)
Add Shipping Rate: 4.86% -> 4.70% (-3.4%, p=0.074)
Two significant declines plus consistent negative direction across all four metrics.Pattern suggests systematic degradation of user experience.

Recommendation: reject variation as negative to business metrics.

Key Insights:

Begin Checkout Rate: most sensitive metric-showed significance in 3/4 tests (both positive and negative).
Add Payment Rate: highest potential impact (+12.5% in Test 1) but inconsistent across tests.
New Account Rate: consistently declining trend-may need separate optimization strategy.
Add Shipping Rate: most stable metric with moderate positive trend.
Further Investigation:

Test 2: determine if null result reflects true ineffectiveness or insufficient test design.
Tests 3 & 4: conduct qualitative analysis (session recordings, heatmaps) to identify specific friction points.
New Account Rate: investigate why this metric consistently underperforms-may need dedicated optimization effort separate from checkout flow.
