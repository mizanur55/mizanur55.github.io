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

