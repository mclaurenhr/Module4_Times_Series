# ML Time Series Modeling (Forecasting)

<img src='Mod4_Pics\pixasquare-4ojhpgKpS68-unsplash.jpg'/>

## Introduction 
In this project I wanted to create a Time Series Model to forecast home values in the Houston, TX area. I decided that I wanted to use the ARIMA modeling method which produced a very accurate prediction model with an RSS score of 0.0001.

I used a Zillow dataset from Kaggle that contained home values in the US from 1996 through 2018. 

This project has been one of my favorite projects to work on to date because of my love for Time Series modeling. I am very interested in forecasting and predictive models that help solve business problems and assist in discovering the best solutions possible to maximizing shareholder's wealth. 

## Data Description
<summary style="font-size: 18px"> Data File Used</summary>

* zillow_data

## Historical Houston Home Values (1996-2018)
<img src='Mod4_Pics\Annotation 2020-08-07 090422.png'/>
<img src='Mod4_Pics\Annotation 2020-08-07 093029.png'/>

## ARIMA Model Results
<img src='Mod4_Pics\download.png'/>

<details><summary style="font-size: 16px"> Question 1: Is it better to invest in fast flips, under 1 year, or hold property for a few years to gain equity before selling?</summary>

<img src='Mod4_Pics\Annotation 2020-08-07 091424.png'/>
<img src='Mod4_Pics\Annotation 2020-08-07 091550.png'/>

#### Question Details 
This question was very straight forward. I wanted to determine if one investment strategy was more profitable over another. I found that investing in fast flip homes that offered a 10%+ a year ROI was better than holding on to homes for a few years before selling. 

</details>

<details><summary style="font-size: 16px"> Question 2: What is the best areas in Houston to invest in?</summary>

<img src='Mod4_Pics\Annotation 2020-08-07 104204.png'/>
<img src='Mod4_Pics\Annotation 2020-08-14 101652.png'/>

#### Question Details
Initially I wanted to investigate into what zipcodes held the most profitable homes in the Houston area to invest in but after conducing my EDA, I realized that I was going to have to compare by counties. Houston has 200+ zipcodes and because of that, I was unable to gather any real substantial findings that way. 

</details>

<details><summary style="font-size: 16px"> Question 3: Is it better to concentrate on investing in one particular area or allocate investing evenly throughout?</summary>

<img src='Mod4_Pics\download (4).png'/>

#### Question Details
I wanted to know if it would be more beneficial if investments were allocated throughout the top 5 counties in Houston or if concentrating in just the top county would bring better returns. I found that there were very little significance in picking one option over the other. Investing soley in Harris county only produced an increase of 0.98% ROI. 

</details>

## Conclusion

There were different time series modeling options I could have used but I decided to use the ARIMA model because it seemed to preform very well. ARIMA stands for AutoRegressive Integrated Moving Average, which is considered a linear regression model, and its a forecasting algorithm based on the information from past values that can be used to predict future values. It is also the most popular model to use in time series modeling.

Me adjusting my p, d, q order from (0, 1, 2) to (2, 1, 2) seemed to help my model fit very well. I had a RSS score of 0.0001 which is very good and translates to producing a variance of no more than $700 off from the original home value and my model's predicted home values.

This notebook is part 1 to my project. I broke up my EDA and my modeling into two different notebooks to keep everything organized. To see my conclusions and business recommendations, go to my part 2 notebook for this project.


## Recommendation
1. When I compared the 1-year home values that gave a return of 10%+ to the 5-year home values, I found the following stats:

##### 1 Year Breakdown @ 10% ROI
1 Year ROI: 13.7%
1 Year Return: $19,223

##### 5 Year Overall:
5 Year ROI: 43.3%
5 Year Return: $66, 807

##### 5 Year Breakdown: 
8.66% Annual ROI
$13,361 Annual Return

I broke the 5 Year overall percentages down into annual, and when you compared the ROI and overall return value between the two, 1 Year ROI of 10%+ seemed to be the best investment option of a ROI of 13.7% and a return value average of $19,223.

In conclusion, it is better to invest in 1 Year fast flips in homes that have brought in an average 10%+ return over holding onto homes for 5 Year to gain equity before selling. 

2. What is the best areas in Houston to invest in?
The best areas to invest in the Houston area is Harris, Galveston, Brazoria, Chambers, and Fort Bent counties. Out of all of the counties, Harris county has the most homes in the area that have a 10%+ yearly ROI. The two areas in Harris county is the Medical Center/3rd Ward area and the Northside area. The Medical Center has a lot of potential with a high value of commuters and local medical professionals desire to live close to where they work. 3rd ward is a historical black neighborhood that has been high hard with the gentrification bug. There are a lot of businesses moving into the area and a lot of homes and neighborhoods actively being renovated. Great investment protential due to the fact that it is a high demand area that is also getting support from the Medical Center area. Northside is another area like 3rd Ward. It is a historically black neighborhood that is starting its gentrification stage. It is a little behind 3rd Ward in development but with it's location between downtown Houston and Bush International Airport, it's another great location with potential. 


3. Investing in Harris county alone or allocating your investments between the other 4 counties really does not make that much of a difference. There is only a difference of 0.98% ROI increase in investing soley in Harris county and a decrease of $763 in home value returns. I recommend an allocation of investments throughout the top 5 counties over Harris county alone.

_____

* Please check out my blog post as well!
<a href="https://medium.com/@heatherrachael9/ml-times-series-modeling-2f39f914adc8">Medium Blog</a>
## Future Work
* I want to look into the expenses side of home investments. My predictions only included profits without any expenses added in. The average home renovation costs are between 3K and 100K with a median of 50K. I want to figure out a good metric for includiing those expenses so that I can have a more realistic outlook on true profits.
* I also want to conduct further research to figureout what the appropriate minimum amount of money is to invest to maximize investors profits. Create a strategy of intelligently selecting the right homes, with the least amount of work needed, to help increase protential profits.
* With Texas being one of the areas in the US that has seen a large amount of growth and epansion, is Houston the best place to invest in? Let's look at investing in Dallas and Austin as well. Are these places growing faster than Houston and do they offer better returns on investments? 