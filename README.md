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

## Next Steps for Analysis:
### 3. Data Cleaning:

- Convert DATE in transaction data to a proper datetime format.
- Standardize and clean PROD_NAME for feature extraction.

### 4. Feature Engineering:

- Extract pack_size (e.g., "175g" → 175).
- Extract brand_name (e.g., "Natural Chip Company SeaSalt" → "Natural Chip Company").

### 5. Merging Datasets:

- Join transaction data with purchase behavior data on LYLTY_CARD_NBR.

### 6. Exploratory Analysis:

- Analyze total sales by LIFESTAGE and PREMIUM_CUSTOMER.
- Examine product preferences by customer segment.

### 7. Insights Derivation:

- Highlight customer segments driving the most sales.
- Identify trends in product and pack-size preferences.

## Insights Based on Analysis
### 1. Sales by Customer Segment
#### Top Performing Segments:
- Older families and older singles/couples contribute the most sales across all premium categories:
      - Older Families: Budget (168,363), Mainstream (103,445), Premium (81,958).
      - Older Singles/Couples: Budget (136,770), Mainstream (133,394), Premium (132,263).

- Retirees and young families also show significant contributions.

#### Target Segments for Growth:
- Young singles/couples in the Premium category represent a smaller contribution (41,642). Strategies targeting this segment could unlock new opportunities.
