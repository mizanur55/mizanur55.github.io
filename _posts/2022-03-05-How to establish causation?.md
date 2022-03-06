---
title:  "How to establish causation?"
mathjax: true
layout: post
categories: media
---




## Introduction
One of the most repeated statistical facts in modern times is “Correlation does not imply causation”. This could be understood by a classic example often given in statistical courses, In the US, the production of ice creams is correlated with number of Drowning deaths as shown by the figure below:

[//]: # (this image below will be centered)
![Alt text](https://raw.githubusercontent.com/mizanur55/mizanur55.github.io/master/_posts/Ice_cream_and_drowning.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

*Fig 1: The correlation between Ice cream production and Drowning in United States*

Does this mean that an increase in Ice cream production cause more drowning? Should we stop producing ice creams to prevent drowning? Well, the answer fortunately is no. Even though these two things are correlated it does not mean they cause each other. So, to put it more simply, when the ice cream production goes up the number of people drowning also happens to increase at the same time but increase in ice cream production does not cause more drowning. It could be that there is a third variable that we have not considered that is responsible for this trend. Consider that in summer as the temperature goes up more people buy ice creams, so this increases the demand for ice creams thus ice cream production goes up. Also, during periods of high temperature more people take up swimming and therefore the likelihood of people drowning also increases. 

From this simple example we can see that it is very important we don’t wrongly derive a causal relationship from a correlation. This could lead us to come to wrong conclusions and in a business setting for example, making decisions based on wrong conclusions could mean that we incur significant losses.


## A Brilliant way of determining causation
Given data about two variables, Correlation between the variables is relatively easy to establish, however, Causation can be extremely difficult, especially given the fact that in the real-world many things affect a variable. This is an area of active research in Statistics and sometimes researchers must come up with clever methods to research causation. In the past, there have been some studies that have been able to study causation successfully. 

In 2005, researchers wanted to see the relationship between police and crime in Washington DC area[[1]](#1). They wanted to answer the question “does more police cause less crime?”. To isolate the effect of “police” on “crime” the researchers found an event where there is an increased police presence for reasons not related to variations in crime. This event was days with high ‘Terror alert levels. Since Washington D.C is the capital, and it is susceptible to terrorist attacks. So, when the terror alert level goes up there are extra police present on many public places, importantly extra police presence on the streets in this case is not because of any variation in crime, it is caused by the threat of terrorism. So, then they asked the question “what happens to level of crime when there are police present for reasons unrelated to crime?”.

The researchers looked at Daily data, rather than a longer time frame as longer time frame data is more prone to endogeneity since it is more likely that over a longer period, we would have explanatory variables that are correlated with error term, when this happens our coefficient estimates $$ (β_i) $$ are less reliable because they are not a true representative of our true coefficients $$ (β_i) $$. They also looked at one city(i.e. Washington DC), this reduces the effect of omitted variables. 

![Alt text](https://raw.githubusercontent.com/mizanur55/mizanur55.github.io/master/_posts/Table_2.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

In Table 2, column (1), we can see that the dummy variable “High Alert” has an estimated coefficient of -7.316, this means that on the days that have High alert levels the total number of crimes decreases by 7.316 crimes on average $$ (±2.877) $$. the $$ R^2 $$ value is 0.14 which indicated that $$ 14% $$ of variability in Daily total number of crimes is explained by High Alert days.

Since the researchers were trying to isolate the effect of “police” has on “crime”, they wanted to consider another variable ‘Metro ridership’ and check whether it could affect crime significantly. The researchers needed to control for Metro ridership as this variable will tell them the number of people in public places(tourism), because if there are less people outside then there are less people on whom the crime can be perpetrated on (i.e. less victims) and this could be the reason which causes lower crime (instead of increased police presence). 

In column (2) of table 2 we observer that the researchers included logged midday ridership along with the High alert dummy variable, we can observe that now we have a smaller coefficient for High alert variable, looking at the estimated coefficients we can also say that a $$ 10% $$ increase in midday ridership increases the daily total number of crimes in DC by 1.7 because $$ 17.341*log (1.10) = 1.7 $$. This suggests that Metro ridership does have a small influence the daily total number of crimes. More simply, if terror threat level causes a decrease in Metro ridership by $$ x% $$ then we expect the crime rate to decrease by <span style="font-size:0.5em;">$$ (17.341*log⁡(1+x/100)) $$</span> all other variables being equal. Since, the daily total number of crimes increase of only 1.7 crimes per day for every $$ 10% $$ increase in Metro ridership is quite small and this increase in not significant, Therefore, the researchers were able to show that they are not wrongly ascribing the crime rate fall due to reduction in metro ridership to “police” numbers. In other words, given their assumption that the metro ridership is a good estimate of tourism, we cannot say that changes in tourists affects daily crime significantly. 

We can also see that the $$ R^2 $$ value has increased to 0.17 which indicated that $$ 17% $$ of variability in Daily total number of crimes is now explained by High Alert days and log(midday ridership). This suggests that by including the midday ridership variable we improved the fit of the model and can explain a higher proportion of the variability. 

## Conclusion
The conclusion here is that from this research we can see that the number of police does affect crime in Washington DC. There seems to be a causal relationship. We have statistical evidence to suggest that the greater the number of police the lower the daily crime in Washington DC. However, we cannot generalise this rule for the entire country as we have not studied the effect of police on crime in other cities. 

In this article, we saw how causation can be established, we also saw that we must take special care when designing our method and may need to come up with uniquely creative way to study causation like in the example I gave in this article, because it can be very difficult to isolate the variables we are studying. With the field of statistics ever evolving, I think that the future in this area looks very interesting and I hope to share more in the future.  



## References
<a id="1">[1]</a> 
Klick, J., & Tabarrok, A. (2005).
Using terror alert levels to estimate the effect of police on crime. 
The Journal of Law and Economics, 48(1), 267-279
  
 


[//]: # (EXTRA - NOTES)

[//]: # (the code below can be used for quotations)
[//]: # (> The secret to creativity is knowing how to hide your sources.) 
[//]: # (&mdash;<cite>[Albert Einstein][1]</cite>)

[//]: # (how to reference: https://stackoverflow.com/questions/26587527/cite-a-paper-using-github-markdown-syntax)

