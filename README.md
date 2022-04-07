# Amazon_Vine_Analysis

## Overview of Project

### Purpose
The purpose of this analysis was to first take a dataset of Amazon review data, transform it using PySpark, then load the created tables into a  PostgresSQL/AWS relational database. Afterwards, the vine data from the review dataset was analyzed for positivity bias. 

## Results
![Vine Analysis](https://github.com/Nveatch/Amazon_Vine_Analysis/blob/main/resources/vine_analysis.png)

**How many Vine reviews and non-Vine reviews were there?**

There were 60 Vine (paid) reviews, and 14,477 non-Vine (unpaid) reviews.
        
**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

There were 34 Vine (paid) reviews that were 5-stars, and 8,212 non-Vine (unpaid) 5-star reviews.

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

Both Vine and non-Vine (paid and unpaid, respectively) reviews has a 5-star review percentage of 57%.

## Summary
From the data, it would appear that there isn't any positivity bias for vine program reviews. As the ratio was 57% for both groups, and not greater for the Vine group, the data shows that unpaid reviewers were just as likely to rate a purchase as 5-stars as their paid counterparts. 

An additional analysis I would perform with the dataset would be similar to this one, but instead of 5 star reviews, I would look at reviews lower than 3 stars. If the unpaid non-Vine reviews had a higher percentage of low ratings (1-2 stars) compared to the paid Vine reviewers, it could indicate there is positivity bias after all. If that were the case, paid reviewers might just be rating bad items slightly higher than the unpaid reviewers, which wouldn't be apparent from just looking at the 5-star reviews.
