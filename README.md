# Quantium-Chips Purchasing Behavior Analysis
## **Overview**
This project analyzes customer purchasing trends and behaviors in the chips category to provide actionable insights for Julia, the Category Manager. The analysis leverages transaction and customer data to identify key patterns, segment customer preferences, and recommend data-driven strategies.

## Technologies Used
- Python: Data analysis and feature engineering.
- Pandas & NumPy: Data manipulation.
- Matplotlib & Seaborn: Data visualization.
- Jupyter Notebook: Interactive environment for analysis.

## Steps to Complete the Analysis:
### Data Cleaning:

#### Remove outliers and incorrect data (e.g., transactions with unusually high or low values).
- Ensure all columns are in the correct data type (e.g., dates, numeric formats).

#### Feature Engineering:

- Derive pack_size from product names (e.g., "Salted Chips 150g" → 150).
- Extract brand_name for product-level analysis.

#### Descriptive Statistics:

- Calculate summary statistics for key metrics like sales and transaction volume.

#### Visualizations:

- Use charts (e.g., bar plots, pie charts) to present findings like: Contribution of each segment to sales and Preferences for pack sizes and brands.

#### Strategic Recommendations:

- Based on the findings, propose actionable strategies for Julia, such as:
    - Focusing on high-value segments.
    - Promoting specific brands or pack sizes to target underperforming segments.
    - Offering discounts on slower-moving products.
 
## Data Sources
- **QVI_transaction_data:** Contains details on purchases, including product names, sales, and quantities.
- **QVI_purchase_behaviour:** Includes customer life stages and premium membership status.

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
### 1. Data Cleaning:

- Convert DATE in transaction data to a proper datetime format.
- Standardize and clean PROD_NAME for feature extraction.

### 2. Feature Engineering:

- Extract pack_size (e.g., "175g" → 175).
- Extract brand_name (e.g., "Natural Chip Company SeaSalt" → "Natural Chip Company").

### 3. Merging Datasets:

- Join transaction data with purchase behavior data on LYLTY_CARD_NBR.

### 4. Exploratory Analysis:

- Analyze total sales by LIFESTAGE and PREMIUM_CUSTOMER.
- Examine product preferences by customer segment.

### 5. Insights Derivation:

- Highlight customer segments driving the most sales.
- Identify trends in product and pack-size preferences.

## Insights Based on Analysis
### 1. Sales by Customer Segment
#### Top Performing Segments:
- **Older families and older singles/couples contribute the most sales across all premium categories:**
      - Older Families: Budget (168,363), Mainstream (103,445), Premium (81,958).
      - Older Singles/Couples: Budget (136,770), Mainstream (133,394), Premium (132,263).

- **Retirees and young families also show significant contributions.**

#### Target Segments for Growth:
- Young singles/couples in the Premium category represent a smaller contribution (41,642). Strategies targeting this segment could unlock new opportunities.

### 2. Pack Size Preferences
#### Popular Pack Sizes (by Sales):
- 110g: Generates the highest revenue, contributing 162,765.
- 134g: Close second with 177,656.
- **Smaller pack sizes like 70g and 90g are less popular, indicating customers prefer medium to large pack sizes.**

### 3. Brand Preferences
#### Top Brands (by Sales):
- Kettle: Dominates with total sales of 390,239.
- Smiths: Second highest with 210,077.
- Doritos: Close third with 201,539.
- Pringles: Also significant at 177,656.
  
These brands likely dominate due to strong brand recognition or premium offerings.

## Strategic Recommendations for Julia
### 1. Focus on High-Performing Segments:

- Retain and deepen engagement with older families and older singles/couples by promoting larger pack sizes or combo deals.

### 2. Opportunities in Underperforming Segments:

- Target young singles/couples in the Premium category through targeted advertising or campaigns emphasizing convenience and indulgence.

### 3. Pack Size Optimization:

- Ensure stock availability for 110g and 134g packs. Consider offering discounts or value packs for these sizes to capitalize on demand.

### 4. Brand Partnerships:

- Collaborate with top-performing brands (Kettle, Smiths, Doritos) for exclusive offers or promotions.
