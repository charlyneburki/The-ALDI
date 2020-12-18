---
title: The ALDI in action 
subtitle: Mapping the index to the London Area
---

# What does the Index result in ? 

Here, we display the optimized weights and the Greater London Area maps that result from the ALDI ranking process. 

![weights](./assets/img/weigths.png){: .mx-auto.d-block :}

We observe that the weights given to each categories have been distributed in such a way that each factor will contribute proportionally to evaluating life. Note also that the **Foods** and **Alcohol** categories have adequate weights to factor in, which is quite nice for our method ! 

We then plot the overall ALDI score, with the weights above, to the Ward level in the Greater London Area and subsequently we aggregate these to the Borough level.

The map :

![ward map](./assets/img/ALDI_ward_map.png){: .mx-auto.d-block :}

It's interesting to note that outer-most wards score genereally better than those close to the City Center. Since this map is quite detailed, we aggregate the data to the Borough level and see which Boroughs perform better: 

The borough-level map:
![borough map](./assets/img/ALDI_borough_map.png){: .mx-auto.d-block :}

It's already easier to read the data ! It also resembles the initial happiness map measuring anxiety and subjective happiness

# Discussion on food 

![borough food map](./assets/img/ALDI_borough_map_foods.png){: .mx-auto.d-block :}

# Want to play around with the weights  ?

We provide sliders for you to customize your index ! You can choose what categories are important to you and attribute them larger weights, and see how the boroughs evolve !

< interactive maps and weights > 
![interactive_map](./assets/img/map.html){: .mx-auto.d-block :}

<iframe
  src="https://raw.githubusercontent.com/charlyneburki/The-ALDI/master/assets/img/map.html"
  style="width:100%; height:600px;"
></iframe>

<div align="center">
  <img src="https://raw.githubusercontent.com/charlyneburki/The-ALDI/master/assets/img/map.html" height="100" />

</div>
