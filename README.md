
# SaaS Product Onboarding & Conversion Analytics

## 📌 Project Overview
This project focuses on product analytics for a SaaS platform, specifically analyzing the user onboarding journey, activation, and monetization. The interactive dashboard tracks key performance indicators (KPIs), monitors registration trends over time, and visualizes the conversion funnel to identify critical bottlenecks where users drop off.

**👉 [View the Interactive Dashboard on Tableau Public](https://public.tableau.com/views/ProductAnalyticsSaaSActivationConversionFunnel/Conversionvisualisation?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**

---

## 🛠️ Tech Stack & Skills
*   **BI Tool:** Tableau Public
*   **Analytical Concepts:** Product Analytics, Cohort Analysis (by registration month), Conversion Funnel Analysis, KPI Dashboarding
*   **Features Used:** Calculated Fields, Dual-Axis Charts, Tooltip Customization, Funnel Charts, Device Layout Optimization

---

## 📊 Key Dashboard Components & Implementation

### 1. High-Level KPI Blocks (Executive Summary)
*   **Registered Users:** Tracks the total number of users entering the onboarding funnel ($8,460$ users).
*   **Trial Users:** Displays the total number of users who activated a trial period ($1,948$ users). 
    *   *Advanced Feature:* Custom tooltips calculate and display the **Registration-to-Trial Conversion Rate** ($23.03\%$).
*   **Paid Users:** Displays the total number of paying customers ($1,384$ users).
    *   *Advanced Feature:* Custom tooltips calculate and display the **Registration-to-Paid Conversion Rate** ($16.36\%$).

### 2. Monthly Registrations & Trial Conversion Trend
A dual-axis chart combining an area chart for absolute registration volume and a line chart for the activation trend. Users are grouped into cohorts by their registration month:
*   Visualizes how many users registered each month (from January to May).
*   Tracks the conversion rate to trial for each monthly cohort, regardless of when the trial actually started. This helps evaluate the impact of product changes or marketing quality over time.

### 3. Conversion Funnel (User Journey Analysis)
A step-by-step conversion funnel visualizing the end-to-end user journey across 5 critical milestones:
1.  `registration` ($100\%$)
2.  `email-verification` ($74.08\%$)
3.  `profile-completion` ($55.08\%$)
4.  `trial-start` ($23.03\%$)
5.  `purchase` ($16.36\%$)

The funnel displays both absolute user counts and relative conversion rates at each stage to pinpoint friction points.

---

## 💡 Key Business Insights (Data-Driven Observations)

*   **The Critical Bottleneck (Onboarding Friction):** The sharpest drop-off occurs between `profile-completion` ($55.08\%$) and `trial-start` ($23.03\%$). The product loses over **$32\%$ of all registered users** at this exact stage. This indicates major friction right before users can experience the product's core value (Aha! moment). *Recommendation:* Optimize the profile setup screen or introduce a skipped/guided onboarding path.
*   **The Early Drop-off:** There is a **$26\%$ loss** immediately after registration before users even verify their email. This could point to issues with email delivery, spam filters, or a tedious verification flow.
*   **High Purchase Intent (Strong Monetization):** Once users actually cross the trial barrier (`trial-start` to `purchase`), the conversion is remarkably high. Out of $1,948$ users who started a trial, $1,384$ upgraded to a paid plan. This represents a **$71\%$ Trial-to-Paid conversion rate**, proving that the product provides strong perceived value once experienced.
*   **Registration & Conversion Dynamics:** While registration volume peaked dramatically in January ($3,673$ users) and steadily declined toward May ($10$ users), the **Registration-to-Trial Conversion Rate remained relatively stable**, fluctuating tightly between $19.36\%$ and $25.59\%$. This suggests that while marketing acquisition slowed down, user quality and baseline product onboarding efficiency remained consistent.
