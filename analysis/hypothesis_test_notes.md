# Hypothesis Test Notes

## Project Information

| Attribute        | Details                                           |
| ---------------- | ------------------------------------------------- |
| Project          | A/B Testing Analysis for User Onboarding Campaign |
| Business Domain  | Subscription-Based Digital Product                |
| Analysis Type    | Controlled A/B Experiment                         |
| Statistical Test | Two-Proportion Z-Test                             |
| Analysis Tool    | Microsoft Excel                                   |
| Date             | July 2026                                         |

---

# Objective of the Hypothesis Test

The objective of this hypothesis test is to determine whether the newly designed onboarding campaign (Treatment Group) produces a statistically significant improvement in User Conversion Rate compared to the existing onboarding experience (Control Group).

The outcome of this statistical analysis will support the business decision regarding whether the new onboarding campaign should be deployed to all users.

---

# Business Problem

The company introduced a redesigned onboarding experience with the expectation of increasing early user activation and improving conversion.

Before implementing the new onboarding flow across the platform, leadership requires statistical evidence demonstrating that the observed improvement is genuine and not the result of random variation.

The experiment compares:

* **Control Group** – Existing onboarding experience
* **Treatment Group** – New onboarding campaign

The statistical analysis provides an objective basis for deciding whether the treatment should be launched.

---

# Metric Being Tested

## Primary Metric

**User Conversion Rate**

---

## Definition

User Conversion Rate represents the percentage of users who successfully complete the desired onboarding objective during the experiment.

It is calculated as:

[
\text{Conversion Rate} = \frac{\text{Number of Converted Users}}{\text{Total Users}} \times 100
]

---

# Reason for Selecting the Metric

User Conversion Rate was selected as the primary evaluation metric because it directly measures the effectiveness of the onboarding experience.

A higher conversion rate indicates that more users successfully complete the activation journey, contributing to business growth through increased product adoption and potential subscription revenue.

Compared with supporting metrics such as Refund Rate or Revenue, Conversion Rate is the most immediate indicator of onboarding success and aligns closely with the company's strategic objective.

---

# Experimental Summary

The experiment randomly assigned users into two groups.

| Group     | Description                    |
| --------- | ------------------------------ |
| Control   | Existing onboarding experience |
| Treatment | New onboarding campaign        |

Random allocation reduces selection bias and ensures a fair comparison between both onboarding experiences.

---

# Experimental Inputs

The statistical test was performed using the following inputs.

| Metric          |   Control | Treatment |
| --------------- | --------: | --------: |
| Users           |   **693** |   **715** |
| Conversion Rate | **3.17%** | **6.99%** |

The observed conversion rate for the Treatment group is substantially higher than that of the Control group, suggesting improved onboarding performance.

---

# Hypothesis Formulation

## Null Hypothesis (H₀)

There is **no statistically significant difference** in User Conversion Rate between the Control and Treatment groups.

[
H_0 : p_{Control} = p_{Treatment}
]

Business Interpretation:

Any observed difference in conversion rates is attributed to random sampling variation rather than the effectiveness of the new onboarding campaign.

---

## Alternative Hypothesis (H₁)

The Treatment onboarding campaign results in a **higher User Conversion Rate** than the existing onboarding experience.

[
H_1 : p_{Treatment} > p_{Control}
]

Business Interpretation:

The redesigned onboarding experience leads to a genuine improvement in user conversion and should be considered for implementation.

---

# Type of Hypothesis Test

## One-Tailed Test

A **one-tailed hypothesis test** was selected because the business objective is to determine whether the new onboarding campaign performs **better** than the current onboarding experience.

The organization is not interested in detecting any difference regardless of direction; instead, it specifically seeks evidence of improvement.

---

# Significance Level

The hypothesis test uses a significance level of:

[
\alpha = 0.05
]

This corresponds to a **95% confidence level**, which is the standard threshold used in business experimentation and product analytics.

A 5% significance level provides an appropriate balance between decision confidence and the risk of making an incorrect recommendation.

---

# Statistical Test Used

A **Two-Proportion Z-Test** was selected because:

* Two independent user groups are compared.
* The primary metric is binary (Converted / Not Converted).
* Sample sizes are sufficiently large.
* The objective is to compare conversion proportions between groups.

The Two-Proportion Z-Test is widely accepted for evaluating conversion-rate experiments in digital products.

---

# Test Output

The statistical analysis produced the following result.

| Metric             |                 Value |
| ------------------ | --------------------: |
| Statistical Test   | Two-Proportion Z-Test |
| Z-Statistic        |             **3.252** |
| Significance Level |              **0.05** |

---

# Equivalent Statistical Evidence

The calculated **Z-statistic of 3.252** exceeds the critical value for a one-tailed test at the 5% significance level.

This provides strong statistical evidence that the observed improvement in User Conversion Rate is unlikely to have occurred by chance.

Although the exact p-value is not reported in the workbook, the Z-score indicates that the p-value is **less than 0.05**, satisfying the predefined significance criterion.

---

# Decision Rule

The decision rule established before conducting the experiment is:

* If the p-value is **less than 0.05**, reject the Null Hypothesis.
* If the p-value is **greater than or equal to 0.05**, fail to reject the Null Hypothesis.

Since the statistical evidence indicates a p-value below the significance threshold, the Null Hypothesis is rejected.

---

# Statistical Decision

**Decision:** Reject the Null Hypothesis (H₀).

The analysis supports the Alternative Hypothesis, indicating that the Treatment onboarding experience significantly improves User Conversion Rate compared with the Control onboarding experience.

---

# Business Interpretation

The statistical findings demonstrate that the redesigned onboarding campaign delivers a meaningful improvement in customer activation.

The increase in conversion is both statistically significant and practically relevant, suggesting that the Treatment experience enables more users to complete the onboarding process successfully.

This improvement has the potential to increase product adoption, subscription growth, and long-term customer value.

---

# Connection to Business Decision

The purpose of the hypothesis test is not only to evaluate statistical significance but also to support an informed business decision.

The experiment provides quantitative evidence that:

* The Treatment campaign outperforms the existing onboarding experience.
* The improvement is unlikely to be due to random chance.
* The primary business objective has been achieved.
* The observed benefits outweigh the limited business risk identified during guardrail analysis.

Consequently, the statistical findings support the recommendation to proceed with the rollout of the redesigned onboarding campaign, while continuing to monitor guardrail metrics after deployment.

---

# Summary

The hypothesis test confirms that the redesigned onboarding campaign achieves a statistically significant improvement in User Conversion Rate.

Using a one-tailed Two-Proportion Z-Test at a 5% significance level, the analysis rejects the Null Hypothesis and concludes that the Treatment onboarding experience performs better than the existing onboarding process.

The statistical evidence, combined with acceptable guardrail performance, provides a strong analytical foundation for recommending the launch of the new onboarding campaign.
