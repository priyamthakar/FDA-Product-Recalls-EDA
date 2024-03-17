# FDA-Product-Recalls-EDA

## Overview
This repository contains an exploratory data analysis of product recalls managed by the FDA. This analysis aims to identify trends and patterns in product recalls over time, across different product types, classification of events, and the distribution of recalls by state and country.


## Data Source
The dataset for this exploratory data analysis, titled `fda_product_recalls.csv`, was sourced from Kaggle, uploaded by [Mexwell](https://www.kaggle.com/mexwell) 
This specific dataset contains information on product recalls issued by the U.S. Food and Drug Administration (FDA) and includes various attributes such as product type, classification, recalling firm, and the state or country of origin.

For more detailed information on the dataset and to download it, visit the following Kaggle page: [FDA Product Recalls](https://www.kaggle.com/datasets/mexwell/fda-product-recalls). The dataset is updated regularly, ensuring the analysis can be conducted with the most recent information available.

Please note that the data provided on Kaggle is for informational purposes only and should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition or product health and safety concerns.



# Key FIndings 
1.	Data Structure & Conversion
- After data type optimization, `product_type`, `product_classification`, `status`, and `recalling_firm_country` were converted to categorical variables for analytical efficiency.
- The dataset reflects a vast spectrum of the recall landscape, with 8,435 unique FEI numbers and 8,839 unique recalling firm names, and a notable 83,124 unique product IDs, showcasing the extensive range and diversity of recall instances. 
2.	Recall Classifications
- Class II recalls were predominant with 59,962 instances, signaling a moderate health impact from the recalled products.
- Class I recalls numbered at 15,421, representing the most severe health risks, while Class III recalls were the least at 7,741, involving minor regulatory infractions.
3.	Product Type Recalls
- Devices had the highest number of recalls at 29,701, indicating a critical need for vigilance in this sector.
- Food/Cosmetics recalls stood at 24,117, while Drug recalls were noted at 15,143.
- Biologics, Veterinary, and Tobacco recalls were comparatively lower at 11,059, 3,096, and 8 respectively.
4.	Geographical Distributions
- The United States had a significantly higher number of recalls at 79,707, with the top states being California (9,078), Florida (5,723), Illinois (4,779), New Jersey (4,318), and New York (4,021).
5.	Temporal Recall Patterns 
- The year 2016 marked the peak in recalls with 8,938 incidents, while 2023 recorded the lowest at 1,910 so far.
- Monthly analysis revealed high recall counts in January (6,481), August (8,051), and December (7,333).
6.	Recall Trends & Status 
- The heatmap of the USA displayed count recalls and indicated geographical hotspots.
- Recall trend analysis highlighted December 2013 as having the highest recall, warranting investigation into specific events or regulatory changes during that time.
7.	Center-Wise and Status-Wise Recall Distribution
- CDRH managed 29,701 recalls, CFSAN handled 24,117, CDER oversaw 15,143, CBER took care of 11,059, CVM had 3,096, and CTP dealt with only 8 recalls.
For recall status, the dataset recorded 131 Class I, 844 Class II, and 56 Class III completed recalls; 1,684 Class I, 9,715 Class II, and 396 Class III ongoing recalls; and 13,606 Class I, 49,403 Class II, and 7,289 Class III terminated recalls.
8.	Recalls in India
- The dataset documented 60 Class II, 13 Class III, and 5 Class I recalls occurring in India.
- Leading recalling firms in India include Mylan Laboratories Limited, Nashik FDF (13 recalls), and Hetero Labs Limited Unit V (9 recalls).
9.	Text Analysis Model Performance
- Precision for recall status classification was excellent, with scores of 1.00 for "Completed," 0.88 for "Ongoing," and 0.90 for "Terminated."
- The model achieved an accuracy of 0.90 across 24,938 support cases but had varying success in recall identification, with an f1-score of 0.13 for "Completed," 0.55 for "Ongoing," and 0.94 for "Terminated."


# Visualizations

## Recalls by Product Classification
- Class I: 15,421 recalls
- Class II: 59,962 recalls
- Class III: 7,741 recalls

## Recalls by Product Type
- Devices: 29,701 recalls
- Food/Cosmetics: 24,117 recalls
- Drugs: 15,143 recalls
- Biologics: 11,059 recalls
- Veterinary: 3,096 recalls
- Tobacco: 8 recalls

## Recalls by Firm Country
- United States: 79,707 recalls
- Canada: 843 recalls
- Germany: 306 recalls
- United Kingdom: 245 recalls
- Switzerland: 243 recalls

## USA

### Top 10 Recalling Firms
- Zimmer Biomet, Inc.: 875 recalls
- OneBlood, Inc.: 713 recalls
- Customed, Inc: 682 recalls
- Garden-Fresh Foods, Inc.: 634 recalls
- Siemens Medical Solutions USA, Inc: 547 recalls
- ICU Medical, Inc.: 539 recalls
- Aidapak Services, LLC: 538 recalls
- American National Red Cross: 519 recalls
- King Bio Inc.: 493 recalls
- GE Healthcare, LLC: 474 recalls

### Top 6 Recalling Firm States
- California: 9,078 recalls
- Florida: 5,723 recalls
- Illinois: 4,779 recalls
- New Jersey: 4,318 recalls
- New York: 4,021 recalls

## Recalls by Year
- 2012: 5,537 recalls
- 2013: 8,562 recalls
- 2014: 7,871 recalls
- 2015: 8,508 recalls
- 2016: 8,938 recalls
- 2017: 7,933 recalls
- 2018: 8,321 recalls
- 2019: 8,274 recalls
- 2020: 6,224 recalls
- 2021: 5,278 recalls
- 2022: 5,768 recalls
- 2023: 1,910 recalls

## Recalls by Month
- January: 6,481 recalls
- February: 6,644 recalls
- March: 6,860 recalls
- April: 6,445 recalls
- May: 6,420 recalls
- June: 6,855 recalls
- July: 7,508 recalls
- August: 8,051 recalls
- September: 6,683 recalls
- October: 6,992 recalls
- November: 6,852 recalls
- December: 7,333 recalls

## Trends of Recalls by Year & Month
- Visual and numerical analysis of recall trends across different times of the year.

## Recalls by Status
- Completed:  1031
- Ongoing: 11795
- Terminated: 70298

## Recalls by FDA Centers
- CDRH: 29,701 recalls
- CFSAN: 24,117 recalls
- CDER: 15,143 recalls
- CBER: 11,059 recalls
- CVM: 3,096 recalls
- CTP: 8 recalls

## Relationship between Product Classification & Status
- Detailed numerical breakdown of recalls by product classification and their respective status.

## Relationship between Product Type & Status
- Analysis and numerical data of the relationship between product type and the current status of recalls.

## For India

### Recalls by Product Type
- Detailed breakdown of product types and their recall counts in India.

### Top 10 Indian Recalling Firms
- Mylan Laboratories Limited, (Nashik FDF): 13 recalls
- Hetero Labs Limited Unit V: 9 recalls
- Shilpa Medicare Limited: 6 recalls
- Hetero Labs, Ltd. - Unit III: 5 recalls
- Lupin Limited: 4 recalls
- Marksans Pharma Limited: 3 recalls
- Alembic Pharmaceuticals Limited: 2 recalls
- Cipla Limited: 2 recalls
- Wockhardt Limited: 2 recalls
- Agila Specialties Private Ltd.: 1 recall

### Recalls by Product Classification in India
- Class II: 60 recalls
- Class III: 13 recalls
- Class I: 5 recalls

### Relationship between Product Classification & Recalling Firm State (Top 5)
- California: Class I (2,018), Class II (6,215), Class III (845)
- Florida: Class I (673), Class II (4,576), Class III (474)
- Illinois: Class I (732), Class II (3,611), Class III (436)
- New Jersey: Class I (496), Class II (3,243), Class III (579)
- New York: Class I (785), Class II (2,781), Class III (455)

# Text Analysis
## Word Cloud of Reason for Recall
- Predominant words: 'product', 'sterility', 'contaminated', 'listeria', 'assurance', 'collected', 'blood', 'CGMP deviation', 'potential', 'distributed'
  
## Word Cloud of Recalling Firm Name
- Most frequent firm names include: 'Zimmer', 'Biomet', 'OneBlood', 'Customed', 'Garden-Fresh', 'Siemens', 'ICU Medical', 'Aidapak', 'American Red Cross', 'King Bio', 'GE Healthcare'
  
## Word Cloud of Product Description
- Common terms found in product descriptions: 'Leukocytes Reduced', 'Apheresis Platelets', 'Red Blood Cells', 'Plasma Source', 'Fresh Frozen', 'Sterile', 'Surgical', 'Packaged', 'Single Use', 'Injection'





