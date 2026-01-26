## A/B Test Analysis: Risk-Aware Onboarding Feature

###  Project Overview

This project analyzes the results of an A/B experiment aimed at evaluating a new risk-aware onboarding feature for an investment platform. The feature provides users with more detailed information about asset risk levels before making deposits. The main goal of the experiment was to understand how improved risk transparency affects user behavior, engagement, and monetization.

The analysis focuses on user conversion, deposit behavior, and revenue-related metrics across control and test groups.

---

###  Experiment Design

* Control group: Standard onboarding without extended risk explanations
* Test group: Enhanced onboarding with detailed risk information
* Users: All registered users, including those who did not make any deposits
* Duration: Full experiment period (daily cumulative analysis included)

---

###  Key Metrics

####  Primary Metric

* ARPU (Average Revenue Per User):
  Average total deposit amount per user, including users without deposits.

####  Guardrail Metric

* Conversion to First Deposit:
  Percentage of registered users who made their first deposit.

####  Secondary Metrics

1. Conversion from First to Second Deposit
2. Average Total Deposit per Paying User
3. Deposit Amount Distribution (25th, 50th, 75th percentiles)

---

###  Key Findings

#### 1. Revenue (ARPU)

* ARPU in the test group increased by ~2.5% compared to control
* The difference is not statistically significant
* Conclusion: The feature did not negatively affect overall revenue per user

#### 2. Conversion to First Deposit (Guardrail)

* Test group conversion was 1.82% lower than control
* The difference is not statistically significant
* Conclusion: The new onboarding does not discourage new users from making an initial deposit

#### 3. Conversion from First to Second Deposit

* Test group shows a ~60% higher conversion rate
* The difference is statistically significant
* Conclusion: The feature significantly improves repeat investment behavior

#### 4. Average Deposit per Paying User

* Test group average is 4.35% higher than control
* Difference is statistically significant
* However, growth is driven primarily by high-value users

#### 5. Deposit Distribution (Bootstrap Analysis)

| Percentile    | Effect               | Interpretation                                            |
| ------------- | -------------------- | --------------------------------------------------------- |
| 25th          | Significant decrease | Small investors became more cautious and reduced deposits |
| 50th (Median) | Moderate decrease    | Typical users show increased risk awareness               |
| 75th          | Significant increase | High-value users increased investments                    |

Conclusion: The feature creates a polarizing effect - it discourages low-risk-tolerant users while encouraging confident, high-value investors.

---

###  Behavioral Insights

* Only 26% of users starting with high-risk assets make a second deposit
* This increases to 43% for medium-risk and 46% for low-risk assets
* Insufficient risk awareness leads to early losses and rapid churn among new users
* Clear risk communication increases confidence and long-term engagement

---

###  Final Conclusion

The risk-aware onboarding feature:

* Improves repeat investments and engagement among active users
* Enhances financial awareness and decision-making
* Does not significantly harm initial conversion
* Strengthens long-term customer value

### Recommendation

Continue optimizing onboarding to balance education and motivation, especially for new users. Improving early risk understanding can reduce churn while preserving growth among high-value investors.

---

### Tools & Libraries

* Python (pandas, numpy, scipy, statsmodels)
* Matplotlib for visualization
* Jupyter Notebook



Data Analysis Project — A/B Testing & Product Analytics
