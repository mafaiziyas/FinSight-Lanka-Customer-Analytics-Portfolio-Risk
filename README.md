# FinSight Lanka - Customer Analytics & Portfolio Risk Assessment

# Predictive Analytics & Risk Management for FinSight Lanka

## Project Overview
This project aims to help FinSight Lanka reduce credit exposure and manage risk across its retail banking portfolio of 500 customers. By analyzing historical dataset records, the goal is to shift from static reporting to identifying structural risk drivers, cross-sell opportunities, and compliance gaps. This provides data-driven strategies to optimize portfolio health across Customer Segments, Loan Types, and Acquisition Channels.

## Main Objectives

### 1. Investigative & Data Preservation Objectives
* **Data Quality Issues:** Audit raw data for contradictions, structural date conflicts, and missing values while applying a maximum data preservation strategy to maintain statistical validity.
* **Exploratory Data Analysis (EDA):** Identify savings, borrowing, and engagement behavior patterns across demographics, acquisition channels, and regions.
* **Key Risk Drivers:** Identify primary variables associated with loan default and high-exposure debt accounts.

### 2. Financial & Risk Exposure Analysis Objectives
* **Quantify Exposure:** Calculate total portfolio savings ($LKR\ 384.60M$) and outstanding credit exposure ($LKR\ 135.0M$ exposed across over-leveraged borrowers).
* **Segment Analysis:** Analyze balance concentration and default variations across Customer Segments (Premium, Regular, Starter) and geographic districts.

### 3. Key Performance Indicators & Monitoring Objectives
* **Risk Benchmarking:** Define and evaluate target metrics for Loan Default Rate ($\le 5.0\%$) and Borrowers Debt-to-Savings Ratio ($\le 40.0\%$).
* **Compliance Monitoring:** Measure Verified KYC Rate ($\ge 95.0\%$) to mitigate anti-money laundering (AML) and regulatory risk.
* **Growth & Engagement Tracking:** Measure 90-day App Active Rates ($\ge 60.0\%$) and Average Products per Active Customer ($\ge 3.00$).

### 4. Strategic & Operational Objectives
* **Mitigation Strategies:** Formulate target credit limit rules, cross-selling initiatives, and digital re-engagement campaigns.
* **Future Data Enhancement:** Justify integrating Credit Bureau (CRIB) data and monthly transaction flows to address proxy analytical limitations.

## 5. Key Insights (EDA Findings)
Based on the analysis of 500 customer records, the following key insights were identified:

* **Savings Concentration:** **63%** of all savings balance ($LKR\ 242.3M$) is concentrated within the Premium segment, despite representing only **18%** of total customers.
* **Credit Risk Alert:** **10.1%** overall default rate across 218 active loans. Vehicle loans (**15.6%**) and Housing loans (**11.4%**) represent the highest default rates.
* **Over-Leveraged Borrowers:** **59.2%** of borrowers (129 customers) owe more than they hold in savings, exposing **LKR 135.0M** (80% of the total loan book value) to severe default risk.
* **Cross-Sell Potential:** **257 customers (51%)** holding **LKR 226.4M** in basic savings do not own Fixed Deposit or Insurance products, representing a prime cross-selling opportunity.
* **Channel Performance:** The Agent channel registered the lowest default rate (**5.4%**), whereas Referral acquisition showed the highest default rate (**12.7%**).

## 6. Methodology
This project follows an end-to-end Data Analytics Lifecycle, structured into five key phases:

### Step 1: Business Context & KPI Definition
* **Problem Definition:** Identified that unmonitored debt-to-savings ratios and low digital/KYC engagement threaten portfolio profitability.
* **Target Metric Benchmark:** Established strict thresholds across 5 core KPIs covering Risk, Compliance, Engagement, and Growth.

### Step 2: Data Engineering & Quality Management
* **Data Preservation (98.4% Retained):** Imputed missing savings balances using Segment + Interest Rate Tier medians instead of dropping records.
* **Conflict Flagging:** Created dedicated audit flags (`Loan_Verified`, `Verified_Adult_Account`, `KYC_Status="Unknown"`) to track future dates and unverified identities without discarding entries.

### Step 3: Exploratory & Portfolio Analysis
* **Univariate & Multivariate Profiling:** Mapped savings distribution across Age Bands (26–45 holding 59% of savings) and Urban/Rural classifications.
* **Risk Mapping:** Linked loan repayment statuses to savings balances to derive true debt-to-savings ratios.

### Step 4: Strategic Recommendations & Modeling Constraints
* **Intervention Design:** Formulated rules to cap loan approval limits against existing savings buffers, prioritizing Starter segment accounts (where 35 of 36 borrowers exceed a 1.0 debt ratio).
* **Cross-Sell Campaign Strategy:** Structured multi-product bundling targeting the 59 liquid Premium accounts with basic savings balances.

### Step 5: Self-Critique & Data Governance Roadmapping
* **Sample Size Validation:** Identified that high-risk segment combinations (e.g., Starter + Vehicle) rest on small sample sizes ($n = 5\text{--}13$) requiring confidence interval tracking.
* **External Integration Plan:** Recommended integrating Credit Bureau (CRIB) scores and monthly income streams for true Debt-to-Income (DTI) assessment.
