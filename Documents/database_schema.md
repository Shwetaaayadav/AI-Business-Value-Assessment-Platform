# Database Schema

## Table 1: Customer_Support

| Column | Type |
|----------|----------|
| ticket_id | INT |
| subject | TEXT |
| body | TEXT |
| answer | TEXT |
| type | VARCHAR |
| queue | VARCHAR |
| priority | VARCHAR |
| language | VARCHAR |

---

## Table 2: Support_Tags

| Column | Type |
|----------|----------|
| tag_id | INT |
| ticket_id | INT |
| tag_name | VARCHAR |

---

## Table 3: Retail_Transactions

| Column | Type |
|----------|----------|
| invoice_no | VARCHAR |
| stock_code | VARCHAR |
| description | TEXT |
| quantity | INT |
| invoice_date | DATETIME |
| unit_price | FLOAT |
| customer_id | VARCHAR |
| country | VARCHAR |

---

## Table 4: Customer_RFM

| Column | Type |
|----------|----------|
| customer_id | VARCHAR |
| recency | INT |
| frequency | INT |
| monetary | FLOAT |
| segment | VARCHAR |

---

## Table 5: Customer_Sentiment

| Column | Type |
|----------|----------|
| ticket_id | INT |
| sentiment_score | FLOAT |
| sentiment_label | VARCHAR |

---

## Table 6: AI_Value_Assessment

| Column | Type |
|----------|----------|
| initiative_id | INT |
| initiative_name | VARCHAR |
| customer_score | FLOAT |
| operational_score | FLOAT |
| financial_score | FLOAT |
| strategic_score | FLOAT |
| final_score | FLOAT |
| recommendation | VARCHAR |