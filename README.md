# Marketing_campaign_analysis_HL


### This document aims to present the test conducted for the analysis of Marketing campaign data.
## The following prompt was provided to carry out the test:

Identify an ad group where performance is suffering because it has a high cost per click (CPC).
Identify an ad group where the RoAS is underperforming compared to the overall campaign’s RoAS during this period, prioritizing by spend.

Identify an ad group that may be experiencing operational issues based on underperforming down-funnel metrics.
Some points to note about the data set:
The actual revenue value was not provided, only the expected revenue. Therefore, an actual_revenue value was created based on the number of conversions, and consequently, the RoAS was calculated using this actual_revenue.

All missing or null values were filled with the mean of the other values (over 77% of records had missing values, so I found it better not to exclude them).

Technologies used: Python (VS Code/Notebook) and SQL for data analysis.


### The answers to the questions are as follows:
## 1.Identify an ad group where performance is suffering because it has a high cost per click (CPC).
The ad group with the highest CPC is AG25, at $7.31, significantly above the average CPC of $2.59. Therefore, this ad group is adversely affecting the overall campaign performance.

## 2. Identify an ad group where the RoAS is underperforming compared to the overall campaign’s RoAS during this time period, prioritizing by spend.
The lowest RoAS belongs to ad group AG33, with a RoAS of 0.016, whereas the average RoAS is 2.7. Consequently, this ad group has the worst performance compared to all others during this time period. All other metrics for this ad group are also below the overall averages.

## 3.Identify an ad group which might be experiencing ops issues based on underperforming down-funnel metrics.
Ad groups AG48 and AG45 show performance issues, with all common metrics (contact rate, referral rate, and referral ms rate) underperforming. (For this analysis, I established thresholds for these metrics, which can be reviewed in the attached code.)

