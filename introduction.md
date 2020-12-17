---
title: an Introduction to ALDI 
subtitle: The Importance of Indexes 
---

# How are people doing ? 

Quality of life has become a increasingly valuable factor in determining policies, governing strategic development and rethinking the way humans evaluate life. A lot of research has gone into improving humans life standard. Recently, indicators such as the [Human Development Index](http://hdr.undp.org/en/content/human-development-index-hdi) (HDI) or customized indices like the [OECD Better Life Index](http://www.oecdbetterlifeindex.org/#/11111111111) have emerged to account for other facets of life instead of simple GDP per capita. The advantages of employing a custom-made index is that a myriad of factors are accounted for, such that we are able to obtain a more accurate reading of “life” and answer the question _"how's life ?"_.

## Why should I care about Indexes ?

Indexes are usually employed to compare countries to one another, allowing organisation such as OECD or the UN to rank countries based on set criteria and produce valuable statistics regarding development and economies. Often, these indexes are included in facts presented to world-wide leaders to set planetary goals with the goal of reducing poverty, hunger and carbon emissions. On a more local level, they can be employed to reflect [housing prices](https://www.homesandproperty.co.uk/property-news/the-best-place-to-live-in-london-revealed-in-new-report-into-the-uks-wellbeing-a124381.html) and much more. Read on to learn how we applied that concept to the Greater London Area !

## Introducing ... ALDI !

Here, we propose a new and improved index to rank, not countries, but local regions in the Greater London Area, in England. More particularly, we look at [Wards](https://en.wikipedia.org/wiki/Wards_and_electoral_divisions_of_the_United_Kingdom) and Boroughs which are both structural localities specific to England. Producing statistics at this level allows, among other things, to read which policies work best in that particular region.  

The ALDI uses standard categories employed in the OECD's ranking:

```markdown
1. Housing
2. Income
3. Jobs
4. Community
5. Education
6. Environment
7. Civic Engagement
8. Health
9. Life Satisfaction
10. Safety
11. Work-Life Balance
```
**and** additionally a **Foods** category and an **Alcohol** category. 

Given the availability of precise food data introduced in the [Tesco Grocery 1.0 ](https://www.nature.com/articles/s41597-020-0397-7) paper at this geographical level, we aimed to explore whether we could extrapolate this data not only to health but to other life indicators. Ultimately, we wanted to see if we could only employ this category to predict happiness/life satisfaction in the Greater London Area -- and see if we could replicate this super acurate map of London Boroughs:

![alt_text](https://github.com/charlyneburki/The-ALDI/blob/master/assets/img/super_accurate_validation_data.jpg)

In fact, much research has concluded that there is an association between eating healthier, varied diets and [higher education](https://www.cambridge.org/core/journals/public-health-nutrition/article/relationship-between-education-and-food-consumption-in-the-1995-australian-national-nutrition-survey/8464FAE847878D59E8D2DD2D06ABB123), converserly more high-fat, caloric diets and [lower education](https://www.sciencedaily.com/releases/2013/11/131106202251.htm), and leading a happier life and [eating healthier](https://link.springer.com/article/10.1007/s11482-019-09748-7#:~:text=Both%20studies%20found%20positive%20correlations,level%20was%20not%20investigated%20longitudinally).  


## But what is an Index and how is it calculated ?

Great question ! In fact, it's important to understand the basics beneath this measurement. An index is made of aggregated data according to different topics. For instance, when we talk about measuring the education level in our dataset, we aggregate data ranging from [GECD](https://en.wikipedia.org/wiki/General_Certificate_of_Secondary_Education) scores to the highest qualification earned when a working adult fills out a census form. These values are then normalized for each to be on the same scale, to allow for unbiased comparaison. Once all the factors for an indicator have been normalized, they must be evaluated for independence, in the sense that they must not be correlated (otherwise we would be giving a factor more weight than necessary). Once we obtain an indicator for all our 12 different categories, we must once more make sure that these factors are not correlated in order to have a most accurate assessment of the life standard.  

To create the ALDI, we followed the recommandations set by the European Union's Joint Research Center in their paper [Tools for Composite Indicators Building](https://publications.jrc.ec.europa.eu/repository/bitstream/JRC31473/EUR%2021682%20EN.pdf?fbclid=IwAR1fziDRyxp6F9B6RAk6wT7pvjBuxs3zV56L-GwR2XYZyczYuDKSd9jy990) in 2005. 

[Let's get to it !](https://charlyneburki.github.io/The-ALDI/aldi/) 




