# Amazon Vine Analysis
Module 16 Challenge Files
- [Amazon_Reviews_ETL.ipynb](https://github.com/aseo67/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)
- [Vine_Review_Analysis.ipynb](https://github.com/aseo67/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)
- [Screenshots](https://github.com/aseo67/Amazon_Vine_Analysis/tree/main/Screenshots)


## Overview of Analysis
This project analyzes reviews from Amazon, in particular those written by members of the paid Amazon Vine program. This program provides products to Amazon Vine members from manufacturers and publishers who pay a fee, and the members in return are required to publish a review. In this analysis, the dataset of Amazon product reviews from the pet product category is extracted, transformed and uploaded to a database. Then, based on further data analysis and exploration, the bias of these Vine reviews is determined. 

## Results
Data Results Screenshot:
![Screenshot](https://github.com/aseo67/Amazon_Vine_Analysis/blob/main/Screenshots/Screenshot%20Vine-NonVine%20counts.png)

- _How many Vine reviews and non-Vine reviews were there?_
  - Number of Vine Reviews: 170
  - Number of non-Vine Reviews: 37,840
- _How many vine reviews were 5 stars? How many non-Vine reviews were 5 stars?_
  - 5-star Vine Reviews: 65
  - 5-star non-Vine Reviews: 20,612
- _What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?_
  - % of Vine Reviews with 5 stars: 38%
  - % of non-Vine Reviews with 5 stars: 54%


## Summary
Based on the results outlined above, there does not seem to be a positivity bias associated with reviews from the Vine program. The percentage of Vine reviews with 5-stars is 38%, which is lower than the percentage of non-Vine reviews with 5-stars (54%). This seems to suggest that usage of the Vine program doesn't inherently bias the reviews positively, resulting in higher ratings. 

One note of caution is that the base size of Vine reviews is much smaller than reviews not from the Vine program. Also, this is specific to the pet product category - some different dynamics might exist depending on the types of products and reviews associated. 

In order to further examine whether there is positivity bias coming from Vine reviews, a couple analyses can further be run: 
- The timing of these Vine reviews and non-Vine reviews with 5-star ratings can be examined. For example, if Vine reviews at the introduction of the product were very positive, this may have influenced subsequent non-Vine reviews to follow the same positive tone, resulting in the high percentage of 5-star reviews. It would be good to gutcheck the timing of these 5-star ratings between Vine and non-Vine reviews (such as through a line plot over time with the frequency of these 5-stars between the two types of reviews). 
- Another gutcheck is to run this same analysis on other categories as well. If we see similar dynamics of non-Vine reviews garnering stronger percentage of 5-star reviews across different product categories, that may suggest that positivity bias from utilizing this program isn't much of a risk - regardless of category. 
