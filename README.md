# Quantium-Chips Purchasing Behavior Analysis
## **Overview**
This project analyzes customer purchasing trends and behaviors in the chips category to provide actionable insights for Julia, the Category Manager. The analysis leverages transaction and customer data to identify key patterns, segment customer preferences, and recommend data-driven strategies.

## **Objective**
The main goal of this project is to:

### - Understand customer purchasing behaviors.
### - Analyze customer segments and their preferences for chips.
### - Derive actionable insights to optimize sales and marketing strategies.

## Data Overview
### 1. Purchase Behavior Dataset (QVI_purchase_behaviour.csv)
Structure:
- 72,637 rows and 3 columns.
- Columns: LYLTY_CARD_NBR (loyalty card number), LIFESTAGE (customer life stage), and PREMIUM_CUSTOMER (premium or budget segment).
**No missing values detected.**

### 2. Transaction Data (QVI_transaction_data.csv)
Structure:
- 264,836 rows and 8 columns.
- Columns: DATE (numeric, needs conversion), STORE_NBR, LYLTY_CARD_NBR, TXN_ID (transaction ID), PROD_NBR, PROD_NAME, PROD_QTY (quantity purchased), and TOT_SALES (total sales).
**No missing values detected.**
