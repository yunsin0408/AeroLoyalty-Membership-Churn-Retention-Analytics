# AeroLoyalty: Membership Churn & Retention Analytics

## Case Study: National Chengchi University (NCCU) Data Analytics Club 5.0 

![K-Means Clustering Plot](da_cover.png)

*Currently the report is only in Traditional Chinese. An English report is in progress.*

📌 Project Overview
This project investigates customer attrition within an airline's loyalty program. By analyzing a dataset of 400k+ flight records and 16k+ members, we developed a predictive understanding of member lifecycles. The goal was to transform raw behavioral data into a segmented retention strategy.

Technical Implementation
1. Data Engineering & Preprocessing
- Feature Construction: Engineered metrics such as Flight Intensity (flights per month) and Point Velocity (rate of accrual vs. redemption).

- Data Integration: Performed joins between relational member profiles and transactional flight logs using Pandas.

- Handling Bias: Addressed class imbalance between active and churned members to ensure model validity.

2. Survival Analysis (The "8-Month Peak")
We utilized Kaplan-Meier Survival Estimators to model the time until a member churns, and identified a critical "Hazard Zone" at the 8-month mark.

This suggests a "Trial Phase" where members lose interest if they haven't achieved a "meaningful win" (e.g., their first redemption) within two fiscal quarters.

3. Machine Learning: K-Means Clustering
We implemented K-Means Clustering to segment the base into four behavioural archetypes:

- Cluster 0 (High-Value Loyal): High frequency, consistent redemption.

- Cluster 1 (High-Risk Churn): Low flight count, zero point usage.

- Cluster 2 (Low-Freq Repurchase): Seasonal travelers with high "dormant" point balances.

- Cluster 3 (Core Stable): Mid-tier travelers with high potential for loyalty "nudging."

📈 Business Impact & Recommendations
- The "First Flight" Nudge: Automated incentives triggered at Month 4 for members with zero redemptions.

- Seasonal Capacity Optimization: Using "Off-Peak" (Spring/Autumn) point multipliers to drive engagement without sacrificing high-demand seat revenue.

- RFM-Based Targeting: Prioritizing retention spend on "Core Stable" members who provide the highest ROI for loyalty intervention.

