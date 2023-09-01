# A/B Testing and Marketing Strategy Analysis for New Fast-Food Item 
## Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Results](#results)
- [Acknowledgments](#acknowledgments)

## Overview

Welcome to the Fast Food Marketing Campaign A/B Test project! This project aims to meticulously evaluate the 
outcomes of A/B testing, enabling us to discern the most effective marketing approach for introducing a new menu item. 
Through a comprehensive exploration of the data, the aim is to make informed decisions that will maximize the impact of 
the marketing campaigns and drive sales growth.

## Data
The dataset for this project originates from a scenario where a fast-food chain is on the brink of introducing a new 
item to its menu. Confronted with the challenge of selecting the optimal marketing strategy, the chain conducted an 
A/B test across various markets. Here's a breakdown of the dataset's key components:

MarketID: A unique identifier for each market.

MarketSize: The market's size, categorized by sales volume.

LocationID: A unique identifier for each store location.

AgeOfStore: The age of the store in years.

Promotion: One of three distinct marketing promotions that were tested.

Week: One of four weeks during which the promotions were executed.

SalesInThousands: The recorded sales amount for a specific LocationID, Promotion, and week.

Examining this dataset aims to uncover the nuanced relationships between market characteristics, store attributes,
promotional strategies, and the resulting sales performance. Through exploratory analysis and data-driven insights, 
the intent is to provide valuable recommendations for shaping the future marketing endeavors of the fast-food chain.

## Results
**1. Initial Data Overview**
Initiated the analysis by examining the dataset, which comprises 548 entries with the following columns:

MarketID: A unique identifier for each market.
MarketSize: The size of the market area categorized by sales.
LocationID: A unique identifier for each store location.
AgeOfStore: The age of the store in years.
Promotion: One of three distinct marketing promotions tested.
Week: One of four weeks during which the promotions were executed.
SalesInThousands: Sales amount for specific LocationID, Promotion, and week.
The dataset is relatively clean, with no missing values and features of different data types.

**2. Promotion Impact on Sales**
The effect of different marketing promotions on sales through the following analyses was assessed:

**Unique Locations:** Observed that each promotion was implemented across a similar number of store locations (Promotion 1: 43 sites, Promotion 2: 47 locations, Promotion 3: 47 locations).

**Summary Statistics:** Examining the summary statistics for sales across different promotions, trends related to market size were identified:

- Large markets had the highest mean sales (Promotion 1: 75.24, Promotion 2: 60.32, Promotion 3: 77.20).
- Medium markets had intermediate mean sales (Promotion 1: 47.67, Promotion 2: 39.11, Promotion 3: 45.47).
- Small markets had the lowest mean sales (Promotion 1: 60.16, Promotion 2: 50.81, Promotion 3: 59.51).
- ANOVA Test: Performed a one-way analysis of variance (ANOVA) to determine if the differences in sales among the three promotions were statistically significant. The results of the ANOVA indicated a statistically significant difference in sales between the promotions (F-statistic: 21.953, p-value: 0.000). This led us to reject the null hypothesis, confirming that at least one promotion had a different effect on sales.

**Tukey's HSD Test:** Conducted Tukey's Honestly Significant Difference (HSD) test to identify pairwise differences in sales between promotions. The results showed that Promotion 1 and Promotion 2, as well as Promotion 2 and Promotion 3, had no significant difference in sales. However, Promotion 1 and Promotion 3 exhibited significant differences.

**Effect Size:** Computed the effect size (η²) for the entire dataset, which revealed a substantial effect of promotions on sales (η² = 0.925).

**3. Market Size Impact on Sales**
Extended our analysis to consider the impact of market size on sales. Key findings for each market size category were as follows:

Large Markets: Promotions had significant differences in sales, with Promotion 3 leading in mean sales.

Medium Markets: Promotions also had significant differences in sales, with Promotion 3 showing the highest mean sales.

Small Markets: Similar to the other market sizes, promotions had significant differences in sales, with Promotion 3 generating the highest mean sales.

**4. Summary**
In conclusion, the analysis demonstrates that the choice of promotion indeed influences sales in the context of this fast-food marketing campaign. Promotion 3 consistently outperformed the other two promotions across different market sizes. Moreover, we observed that market size had a noteworthy impact on sales, with large markets generally achieving higher sales figures.

These insights are pivotal for the fast-food chain's marketing strategy, as they can guide decisions on which promotion to adopt for specific market sizes to maximize sales and profitability.


## Acknowledgments

The dataset was made available through various sources:

- https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test?resource=download
- [RPubs](https://rpubs.com/ksdwivedy/finalRProject)
- "Hands-On Data Science for Marketing" book by Yoon Hyup Hwang
- [Unsplash](https://unsplash.com/@shaafi) for the cover image
- IBM Watson Analytics community for providing this dataset.

