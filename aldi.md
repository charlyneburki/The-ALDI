---
title: Diving into the Categories 
subtitle: A showcase of what is contained in some of the indicators
---

# An Overview of some Important Categories

Let's take a look at a few indicators to understand what is contained in them and what we are measuring !

## Foods 

First up, it's important to understand what is inside the `Foods` category. What are people buying ? What are people eating ? 

We answer this question by plotting the frequency of the different categories of food contained in our dataset. We see that people tend to buy a lot more fruits and vegetables than any other categories. We also see that animal products do not make up a large part of consumer's diets. It's interesting to note that despite having busy lives, ready-made foods do not figure in the top purchased food items.  

<insert the first graph for food >

This heatmap shows us a lot about general nutrition. Fibers are found mainly in fruits and vegetables, as higlighted by the relatively strong correlation between fibers energy and fruits & vegetables. It's suprising to see that ready-made items correlate negatively with fibers energy, meaning that because we inversed the first variable, they actually correlate positively ! Also areas that buy larger fractions of sweets obtain higher counts of energy from fats, sugar and carbs.

<insert the second graph for foods>
![foods](./assets/img/exploring_foods.png){: .mx-auto.d-block :})

Thus, the food indicator is made of a diverse set of food items and measures that also presents normal correlation factors.

## Environment 

This next category is all about measuring the condition of the environment.

![env](./assets/img/exploring_env.png){: .mx-auto.d-block :}

Though the two indicators for air pollution ([PM10](https://www.eea.europa.eu/data-and-maps/indicators/emissions-of-primary-particles-and-5/assessment-3#:~:text=UNECE%20LRTAP%20Convention.-,PM10%3A%20Particulate%20matter%20(particles%20with%20diameter%20of%2010%20micrometres%20or,by%20European%20Environment%20Agency%20(EEA) emissions and [NO2](https://www.epa.gov/no2-pollution#:~:text=NO2%20primarily%20gets%20in,%2C%20and%20off%2Droad%20equipment)) emissions may appear to be highly correlated from the heatmap, they measure different pollutions at different levels. In fact, we see that PM10 pollution spans a diffferent range from that of NO2 emissions. NO2 emissions also have higher levels and about 10 percent of the London areas are above the [norm](https://www.who.int/news-room/fact-sheets/detail/ambient-(outdoor)-air-quality-and-health) set by the World Health Organisation, which indicates poor air quality. 

The two air pollution indicators are also correlated relatively strongly to the `percent of greenspace area`. This suggests that the two indicators may also, to a certain extent, express how much green space there is (remembering that we inversed that variable). 

We can see that lots of areas have a positive relative variable distribution, the variable being inversed, this means all those areas have quite good air quality. and will have a small score boost (due to a combination of having a slightly positive value and a small weight for those variables). In contrast a small number of areas have a very bad air quality (on the left of the graph), and thus will be quite strongly penalized (big negative value but still small weight).

Another example is with homes_without_access_nature_%, we see that most areas have a small percentage of homes without access to nature (again let's not forget that this data was inversed). So they have a relatively small score boost, but the ares that have a big percent of homes without access to nature get penalized strongly.

Finally area_greenpace_% has a reltively small number of areas with a high percentage of greenspace (rigth of graph), these areas are stronly boosted (relative positive score and big weigth), but the others, which have a small percent of greenspace, will be penalized quite strongly (but not too much, as they have a relatively small negative score).

## Sounds easy right ? But ... 

This was a brief overview of what is contained in our subcategories. This data is actually rescaled and normalized and sometimes inversed in order to compare the different values on the same scale. Evidently, we cannot compare the pollution emitted via particle counts to a count of violent incidents happening ! 

Once we rescale all our data we obtain independent indicators, as showcased here in this heatmap :

< inlcude heatmap of all indicators> 

As we can observe by the colors, all our indicators are independent of one another, which is an essential criterion for producing an index that reflects different aspects of life evaluation. 

After that, we looked to optimize the weights attributed to each category. That is, we employed Principle Component Analysis (PCA) to determine the directions that contain the most variance, and assigning them more important weights. This process allows us to **optimize** the weights. In the end, we obtain an index containing the weights of each indicators such that they optimally represent the data we have and reflect most accurately what is going on in the Greater London Area. 

[Let's find out the results !](https://charlyneburki.github.io/The-ALDI/map/) 

