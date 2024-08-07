# A/B-Testing
A/B Testing on conversion rate

**Overview**

This project involves conducting an A/B test to evaluate the effectiveness of a new landing page design compared to the old design. The goal is to determine if the new design (treatment group) leads to a higher conversion rate compared to the old design (control group).

**Project Components**

Data Source: Kaggle A/B Testing Dataset
Key Metrics:
Conversion Rate
Confidence Intervals
Statistical Significance

**Dataset**

The dataset includes information about user interactions with two versions of a landing page. Key columns used in this analysis include:

group: Indicates the experimental group (control or treatment).
converted: Binary column indicating whether the user converted (1) or not (0).
landing_page: The version of the landing page viewed by the user (old or new).

**Data Preprocessing**

The dataset was cleaned to ensure accurate analysis. This included:
1)Checked for missing values
2)Removed users who have been sampled multiple times (to avoid skewed results.)
3)identify the ideal sample size based on power and alpha value.


**Data Sampling:**

Sampled the necessary number of users for the control and treatment groups to ensure statistically valid results.

**Hypothesis Testing:**

**Null Hypothesis (H0):** There is no significant difference in conversion rates between the control group (old landing page) and the treatment group (new landing page).

**Alternative Hypothesis (H1):** There is a significant difference in conversion rates between the control group and the treatment group.

**Statistical Analysis:**

1)Performed statistical tests (Z-test and T-test) to compare conversion rates between the control and treatment groups.

2)Confidence Intervals: Calculated 95% confidence intervals for the conversion rates to understand the range within which the true conversion rates are likely to fall.

3)Visualization:Created visualizations to compare conversion rates between control and treatment groups.

**Results**

**Conversion Rates:**

Control Group: **12.33%** (95% CI: [11.42%, 13.30%])
Treatment Group: **12.56% **(95% CI: [11.65%, 13.54%])
Statistical Tests:

Z-Test: Z-Statistic: -0.3430, P-Value: 0.7316
T-Test: T-Statistic: -0.3429, P-Value: 0.7317
**Conclusion**

The analysis indicates no statistically significant difference between the conversion rates of the control and treatment groups. With p-values well above the common alpha level of 0.05, we fail to reject the null hypothesis. The confidence intervals for both groups overlap, suggesting that the new landing page does not lead to a significant improvement in conversion rates compared to the old one.

**Further Work**

Explore Other Factors: Investigate additional variables or factors that might influence conversion rates.
Run Additional Tests: Consider running more experiments or exploring different variations of the landing page.

**License**
This project is licensed under the MIT License
