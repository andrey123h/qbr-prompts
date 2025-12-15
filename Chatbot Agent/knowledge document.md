**Internal Knowledge Base — Customer Success Analytics**

---

## 1. Purpose & Usage

This document defines the **official company policy** for interpreting **Quarterly Business Review (QBR) metrics**.  

---

## 2. Core Account Fields 

These fields are the **raw inputs** used for QBR analysis.

### 2.1 Account & Subscription

| Field | Description |
|---|---|
| `account_name` | Customer name |
| `plan_type` | Subscription type |

### 2.2 Usage & Adoption

| Field | Description |
|---|---|
| `active_users` | Number of active users |
| `usage_growth_qoq` | % change in usage quarter-over-quarter |
| `automation_adoption_pct` | Automation feature adoption rate |

### 2.3 Support & Satisfaction

| Field | Description |
|---|---|
| `tickets_last_quarter` | Support ticket count |
| `avg_response_time` | Average support response time (hours) |
| `nps_scorz` | Most recent NPS score |

### 2.4 Health & Risk

| Field | Description |
|---|---|
| `scat_score` | Success Confidence & Adoption Trend (SCAT), 0–100 |
| `risk_engine_score` | AI-predicted churn risk (0–1, higher = riskier) |

### 2.5 Qualitative Inputs

| Field | Description |
|---|---|
| `preferred_channel` | Main communication preference |
| `crm_notes` | Qualitative notes from the CSM |
| `feedback_summary` | Key feedback or feature requests |

---

## 3. Metric Categorization Policies 

All labels below are **business-approved interpretations**.

---

### 3.1 Usage Growth (Quarter-over-Quarter)

**Metric:** `usage_growth_qoq`

| Range | Label | Interpretation |
|---|---|---|
| ≥ 0.30 | **Outstanding Growth** | Exceptional expansion and strong value realization |
| ≥ 0.15 | **Strong Growth** | Healthy and accelerating adoption |
| ≥ 0.05 | **Moderate Growth** | Positive but slower momentum |
| ≥ −0.05 | **Stable / Flat Usage** | No significant change |
| ≥ −0.15 | **Mild Decline** | Early signs of reduced engagement |
| ≥ −0.30 | **Moderate Decline** | Concerning usage drop |
| < −0.30 | **Severe Decline** | Critical contraction |

**Policy note:**  
Usage growth is a primary signal for expansion and renewal conversations.

---

### 3.2 Automation Adoption

**Metric:** `automation_adoption_pct`

| Range | Label | Interpretation |
|---|---|---|
| ≥ 0.70 | **High Adoption** | Strong platform leverage |
| ≥ 0.40 | **Moderate Adoption** | Partial feature usage |
| ≥ 0.20 | **Low Adoption** | Limited automation value |
| < 0.20 | **Very Low Adoption** | High enablement opportunity |

---

### 3.3 Support Ticket Load

**Metric:** `tickets_last_quarter`

| Range | Label | Interpretation |
|---|---|---|
| ≤ 5 | **Very Low Ticket Load** | Minimal friction |
| ≤ 15 | **Low Ticket Load** | Healthy support usage |
| ≤ 30 | **Moderate Ticket Load** | Manageable friction |
| ≤ 60 | **High Ticket Load** | Operational strain |
| > 60 | **Critical Ticket Load** | Escalation required |

---

### 3.4 Support Response Time

**Metric:** `avg_response_time` (hours)

| Range | Label | Interpretation |
|---|---|---|
| ≤ 2 | **Excellent Response Time** | Best-in-class support |
| ≤ 6 | **Good Response Time** | Acceptable SLA |
| ≤ 12 | **Slow Response Time** | Risk of dissatisfaction |
| > 12 | **Very Slow Response Time** | High churn sensitivity |

---

### 3.5 Net Promoter Score (NPS)

**Metric:** `nps_scorz`

| Range | Label | Interpretation |
|---|---|---|
| ≥ 9 | **Promoter** | Strong advocacy potential |
| ≥ 7 | **Passive** | Neutral satisfaction |
| < 7 | **Detractor** | Dissatisfaction risk |

**Policy note:**  
NPS labels must not be softened or rephrased.

---

### 3.6 SCAT — Success Confidence & Adoption Trend

**Metric:** `scat_score`

| Range | Label | Interpretation |
|---|---|---|
| ≥ 85 | **Very Healthy** | Strong long-term outlook |
| ≥ 70 | **Healthy** | Stable account |
| ≥ 50 | **At Risk** | Requires CSM attention |
| < 50 | **Critical Risk** | Immediate intervention needed |

---

### 3.7 Churn Risk (AI-Predicted)

**Metric:** `risk_engine_score`

| Range | Label | Interpretation |
|---|---|---|
| ≥ 0.90 | **Critical Churn Risk** | Immediate escalation |
| ≥ 0.75 | **Very High Churn Risk** | Executive attention |
| ≥ 0.45 | **High Churn Risk** | Proactive mitigation |
| ≥ 0.25 | **Moderate Churn Risk** | Monitor closely |
| ≥ 0.10 | **Low Churn Risk** | Stable |
| ≥ 0.03 | **Very Low Churn Risk** | Strong retention |
| < 0.03 | **Minimal Churn Risk** | Extremely safe |

---

