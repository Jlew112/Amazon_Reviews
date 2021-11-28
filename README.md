# Amazon_Reviews

## Overview
For this analysis, our goal was to check the Amazon Vine program for bias. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products for a small fee. The concern being that if reviewers have monetary incentive to review the products, will the reviews be positively biased?

We chose the video game review data to run our analysis. The goal is to find the total number of reviews; filter the the number of useful reviews; then breakdown the star counts for reviews from vine (vine) based reviewers, and non-vine (unpaid) based users.

## Results
Here are the results of our breakdown:
- Total Reviews = 1785997
- Total Reviews with atleast 20 votes = 65379
- Total Reviews with a helpful rating at or above 50% = 40565
- Total helpful reviews from the paid reviewers (Vine) = 94
- Total helpful reviews from the unpaid reviewers (no Vine) = 40471

With our totals lined out, it is time to check the star ratings from each group.
![alt text](https://github.com/Jlew112/Amazon_Reviews/blob/main/helpful%20total%20star%20breakdown.PNG?raw=true)
![alt text](https://github.com/Jlew112/Amazon_Reviews/blob/main/no%20vine%20star%20breakdown.PNG?raw=true)
![alt text](https://github.com/Jlew112/Amazon_Reviews/blob/main/yes%20vine%20star%20breakdown.PNG?raw=true)

I've highlighted the area where I expect to see the biggest issue. 1 Star votes. 
- Total helpful reviews percentage of 1 star: 25% 
- Total unpaid reviews percentage of 1 star: 25%
- Total paid reviews percentage of 1 star: 1%
- Total helpful reviews percentage of 5 star: 39% 
- Total unpaid reviews percentage of 5 star: 39%
- Total paid reviews percentage of 5 star: 51%

## Summary
As we can see in the data, there is certainly a skew in the reviews. Not only are more vine reviewers (proportionately) giving 5 star ratings, but they are also giving far fewer  1 star reviews. The data suggests that the paying for reviews will, most likely, provide more positive reviews. Unfortunately, those positive reviews may not be in the consumer's best interest. For additional analysis, we should use regular expressions to try to find reviews that specifically reference past reviews, ex: "I bought this because the past reviews were great! But boy were they wrong." Or "I'm glad I listened to the reviews!" if we check the star ratings based on that criteria, I'd be curious to see if consumers actually find the reviews useful or not.
