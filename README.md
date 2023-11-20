## Hypothesis Testing

![Problem](https://github.com/hayasalman/Hypothesis-Tests/assets/71796909/c7ff2780-e8e4-4667-be1a-727905833dcb)

## Overview 

According to Jim Frost , the hypothesis testing is a form of inferential statistics that allows us to draw conclusions about an entire population based on a representative sample.

In most cases, it is simply impossible to observe the entire population to understand its properties. The only alternative is to collect a random sample and then use statistics to analyze it.

In this repository there are different types of hypothesis tests performed on different samples.

## About The Dataset

- All the samples stored as CSV file and can be accessed through this links :

  - **Transportation Sample** : [Trips Duration Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/transportion_data.csv)
  - **Sodium Levels Sample** : [Sodium Levels](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/sodium_data.csv)
  - **TCS Marathon Sample** : [Participants Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/runners_data.csv)
  - **Fine Dining Restaurants Ratings Samples** : [Restaurant A Ratings](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/restaurant_A_ratings.csv) - [Restaurant B Ratings](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/restaurant_B_ratings.csv)
  - **Nutrition App Sample** : [Weights Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/nutrition_data.csv)
  - **Movies Preferences Sample** : [Preferences Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/movies_pref.csv)
  - **US & India Chocolate Rating Scores Sample** : [Chocolate Scores](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/chocolate_scores.csv)
  - **Espresso Caffeine Content Sample** : [Caffeine Content Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/caffeine_content_mg.csv)
  - **Advertisements Sample** : [Ads Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/ads_samp.csv)
  - **UEFA Champions League Sample** : [UCL Champions Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/UEFA_Champions_League_Sample.csv)
  - **NYSE Stock Prices Sample** : [Stock Prices Info](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Samples/NYSE_stock_prices.csv)
 
  ## Coding

  -  Python Integrated Development Environment (IDE) : Jupyter Notebooks.

   **Packeges used** 
  * **pandas - numby** : used for data manipulation.
  * **matplotlib - seaborn** : used for data visualtion.
  * **scipy** : used for hypothesis tests.
 
  ## Approaches & Methodologies

  1. Define the business problem.
     
  2. State the Null Hypothesis which is denoted by this symbol *H0* and the Alternative Hypothesis which is denoted by this symbol *Ha*.
 
  3.  Pre-set the level of statistical significance (alpha) α, and we should set α before the experiment (a prior).
 
      - There are two types of errors we should avoid :
      
         - **Type I Error (FP) OR α (alpha)** : reject null hypothesis, when it 's actuatly true.
         - **Type II Error (FN) OR β (beta)** : fail to reject null hypothesis, when it's actuatly false.This error rejects the alternative hypothesis, even though it does not occur due to chance.

      -  The typical value of α is 0.05, establishing a 95% confidence level, so we allow only 5% as the maximum chance of incorrectly rejecting the null hypothesis, and this is what we will be 
         using for all the tests. 
         Moreover, if we want to be more precise about the test result we can set the significance level to 0.01, with a 99% confidence level in which we only have 1%  chance to be wrong when we 
         strongly believe that the null hypothesis to be true and the alternative hypothesis happens due to pure chance and there's no statistical evidence to support it unless it's true and 
         didn't only falsely impacted by the slight differences.
         But in some cases, we may end up minimizing the risk of the Type I error by reducing the level of significance and widthen the confidence interval bounds, but at the same time we risk 
         making Type II error as well.

       
    4. Collect the data.
 
    5. Select the proper test.

        1. One Sample Z-test.
        2. One Sample T-test.
        3. Two Independent Sample Test.
        4. Paired Samples T-test.
        5. Proportion Z-test.
        6. F-Test.
        7. Chi-Square Tests.
        8. One-way Anova Test.
 
    6. Calculate a test statistic.
 
    7. Construct acceptance / rejection regions OR find the P-value.
 
    8. Draw conclusions.
 
  ## Business Insights

  These are some of the intersting insights we found after analyze the tests result.

- In case of [The Airlines Company](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One%20Sample%20Z-test.ipynb). The company actually should start to 
  worry about the increment in the mean flight time and investigate more about the reasons that led to this and that doesn't happen due to extremes in the sample drawn. As the drawn sample may 
  contain some of historical casual accidents that led to this result, in this situation they can draw another sample and do the test again , but if they come up with the same result that means 
  the company does have some serious issues that cause this slipping in the mean flight time.

- In case of [The Shampoo Bottles Manufacturing Company](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One%20Sample%20Z-test.ipynb). There are two 
  different statements about the shampoo amount at each bottle, one made by the quality control team of the shampoo manufacturing company and the other is a claim made by one of its customers. 
  First, about the quality control team statement we found that it's not necessarily the mean amount of shampoo in the bottles that is exactly 250 ml , and in fact it's less than the mean 
  amount by **-1.92** , but since that does not a significant observed difference in order to the quality team take it in consideration.
  For the customer claim , the quality team already knew that the customer was right about his/her claim from the result of the previous hypothesis test , the mean amount of the shampoo in the 
  bottles is not necessarily exactly 250 ml and it could differ from bottle to other. However, since they are not below the mean amount of 250 ml by significant observed difference, then 
  there’s no need to start to be worried.

- In the case of [The Transportation Company](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One%20Sample%20T-test.ipynb) which advertised that within a 
  radius of 5 km from the pickup to the destination , they will apply discount coupons for these trips as long the trip duration doesn't exceed 15 minutes in order to retain the business against 
  the stiff competition from its main rival. And the company was right about the mean trip duration within a 5 km radius it usually don't take more than 15 minutes , even if we observed that some 
  trips might be slightly more than 15 minutes due different factors such as : the traffic, the day of week,......,etc , but not more than 5% of the mean trip duration.

- In the case of [The Dark Chocolate Scores](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Two%20Independent%20Sample%20Test.ipynb) with 95% confidence 
  we say that dark chocolate is more popular in the US than in India based on the scores.

- In the case of [The Next UCL Champion](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Proportion%20Z-test.ipynb) we don't have enough statistical 
  evidence to say that Real Madrid will be the next UCL champion , even though Real Madrid is the most successful club so it's reasonable to assume that this claim is true. However , there's 
  still a possibility of 24% that Real Madrid will win the next season, but it's not certain or guaranteed.

- In the case of [The Movies Prefrences](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Chi-Square%20Tests.ipynb) we have enough statistical evidence to 
  come up with that the movie preferences depend on marital status.

## References

- [One Sample Z-Tests File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One%20Sample%20Z-test.ipynb)
- [One Sample T-Tests File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One%20Sample%20T-test.ipynb)
- [Two Independent Samples Tests File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Two%20Independent%20Sample%20Test.ipynb)
- [Paired Samples Tests File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Paired%20Samples%20T-test.ipynb)
- [F-Test File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/F-test.ipynb)
- [Chi Square Tests File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/Chi-Square%20Tests.ipynb)
- [One-way ANOVA Test File](https://github.com/hayasalman/Hypothesis-Tests/blob/main/Hypothesis%20Testing%20Notebooks/One-way%20Anova%20Test.ipynb)

  
   
             

      
