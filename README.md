# Fandango-Movies-Rating-Investigation

In October 2015, a data journalist named Walt Hickey analyzed movie ratings data and found strong evidence to suggest that Fandango's rating system was biased and dishonest (Fandango is an online movie ratings aggregator). He published his analysis in this article

Fandango displays a 5-star rating system on their website, where the minimum rating is 0 stars and the maximum is 5 stars.

Hickey found that there's a significant discrepancy between the number of stars displayed to users and the actual rating, which he was able to find in the HTML of the page. He was able to find that:

The actual rating was almost always rounded up to the nearest half-star. For instance, a 4.1 movie would be rounded off to 4.5 stars, not to 4 stars, as you may expect.
In the case of 8% of the ratings analyzed, the rounding up was done to the nearest whole star. For instance, a 4.5 rating would be rounded off to 5 stars.
For one movie rating, the rounding off was completely bizarre: from a rating of 4 in the HTML of the page to a displayed rating of 5 stars.

From the graph in an article we can see that both distributions above are strongly left skewed, suggesting that movie ratings on Fandango are generally high or very high. We can see there's no rating under 2 stars in the sample Hickey analyzed. The distribution of displayed ratings is clearly shifted to the right compared to the actual rating distribution, suggesting strongly that Fandango inflates the ratings under the hood.


Fandango's officials replied that the biased rounding off was caused by a bug in their system rather than being intentional, and they promised to fix the bug as soon as possible.


The aim of this project is to analyze more recent movie ratings data to determine whether there has been any change in Fandango's rating system after Hickey's analysis.

Data to analyze the characteristics of Fandago's rating system previous to Hickey's analysis used for this project has been collected by Walt Hickey and is available [here](https://github.com/fivethirtyeight/data/tree/master/fandango).

To analyze the rating system's characteristics after Hickey's analysis we will be using the data for movies released in 2016 and 2017 from [here](https://github.com/mircealex/Movie_ratings_2016_17)
