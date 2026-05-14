SaaS Customer Behavior & Revenue Analysis
Overview

This project is a SaaS product analytics case study focused on understanding how customers behave across the full lifecycle of a subscription-based platform — from acquisition and engagement to support interactions and eventual churn.

Instead of treating this as isolated SQL queries, the analysis is framed as a connected business study aimed at understanding how revenue, engagement, and customer experience interact to drive retention outcomes.

Dataset Overview

The dataset represents a relational SaaS system where multiple tables are connected through unique identifiers, enabling customer-level tracking across the entire lifecycle.

It includes:

500 customer accounts
5000 subscription records
feature usage logs capturing product interactions
support ticket data reflecting customer experience
churn event data with reason-level classification

Together, these datasets allow analysis of how users behave inside the product, how revenue is distributed, and what patterns are associated with churn.

Problem Statement

The goal of the analysis was to understand how users behave inside a SaaS product and what drives outcomes like revenue growth, retention, or churn.

More specifically, the focus was on understanding how subscription tiers perform, how engagement varies across users, whether usage patterns can predict churn, and how support experience fits into the overall customer journey.

Key Areas of Analysis

Revenue was analyzed across subscription tiers to understand where value is concentrated and how customer movement through upgrades and downgrades affects overall revenue.

Product engagement was studied to identify which features drive usage and whether beta feature adoption correlates with stronger retention.

Retention behavior was analyzed using cohort tracking and stickiness metrics (DAU/MAU) to understand how consistently users return to the platform.

Churn analysis focused on both behavioral comparisons and structured churn reasons to identify patterns behind customer loss.

Support data was included to evaluate whether ticket volume, resolution time, and satisfaction scores influence churn behavior.

Key Insights
Revenue is heavily concentrated in higher subscription tiers, indicating that a smaller group of users drives most of the monetization.
Beta feature users show stronger retention and upgrade behavior compared to non-beta users, suggesting deeper product adoption improves customer value.
Engagement alone is not a strong predictor of churn — churned and active users often show similar usage patterns.
This suggests that churn is less about activity and more about perceived product value or customer expectations.
Support experience metrics (resolution time, satisfaction scores) show a stronger relationship with churn than raw usage metrics.
Overall, retention appears to depend more on qualitative experience than on usage volume alone.

Data Challenges & Handling

A few practical issues were handled during the analysis:

boolean fields were stored as text and normalized directly in SQL
time-based fields required conversion for cohort and trend analysis
joins across multiple tables were carefully structured to avoid duplication
usage metrics were standardized for consistent comparison across segments

Tools Used
PostgreSQL (primary analysis engine)
SQL (joins, aggregations, CTEs, CASE logic, cohort analysis)
PowerPoint (visual storytelling and presentation of SQL outputs)
Excel (used for quick validation and organizing aggregated results)

Business Impact

This analysis can help a SaaS business better understand which customers are most valuable, which behaviors signal churn risk early, and how product or support improvements might improve retention.

It also highlights that retention is not just a function of usage, but also strongly influenced by customer experience and perceived value.

Visual Summary

Some SQL outputs were converted into charts in PowerPoint to visually represent key patterns such as revenue distribution, cohort retention trends, and churn comparisons.

These visuals were used to support storytelling and make analytical findings easier to interpret.

Conclusion

This analysis shows that SaaS customer behavior is multi-dimensional and cannot be understood through usage metrics alone.

While engagement is important, retention is more strongly influenced by customer experience, support quality, and perceived value.
