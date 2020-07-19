# E-commerce-Product-Recommendations---Recommendation-System

## Context

This dataset taken from [Kaggle](https://www.kaggle.com/cclark/product-item-data). 

## Overview

A simple Recommendation system involving a content-based filtering, using Cosine Similarity and Jaccard Similarity. A summary results can be seen below, but for details can be seen in [this notebook](https://github.com/Stev-create/E-commerce-Product-Recommendations---Recommendation-System/blob/master/E-Commerce%20Product%20Recommendation.ipynb).

### Summary

#### Exploratory Data Analysis

First, I need to clean the data. As we can see below the random sample show us there is tags HTML like `<br>`, `<b>`, `<ul>`, etc.

![GitHub Logo](/images/cos1.png)

And after that, I'm curious about the distribution of length of the description. So I visualize it, 

![GitHub Logo](/images/cos2.png)

The distribution show us, that the seller's strategy its good. The description shouldn't be too long. After that, i want to know what words often appear in this dataset. I'm using word cloud to answer that question, that we can see below:

![GitHub Logo](/images/cos3.png)

Oh, That's make sense. Because when we see the description of the dataset, it said "500 actual SKUs from an outdoor apparel brand's product catalog." Thats why, there is many clothing material words and many product is an eco-friendly clothes. 

#### Cosine Similarity & Jaccard Similarity

Cosine Similarity has a simple equation

<a href="https://www.codecogs.com/eqnedit.php?latex=similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?similarity&space;=&space;\cos(\theta)&space;=&space;\frac{\vec{A}\cdot&space;\vec{B}}{\left&space;|&space;A&space;\right&space;|\left&space;|&space;B&space;\right&space;|}" title="similarity = \cos(\theta) = \frac{\vec{A}\cdot \vec{B}}{\left | A \right |\left | B \right |}" /></a>
 
While Jaccard Similarity equation is

<a href="https://www.codecogs.com/eqnedit.php?latex=J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?J(A,B)&space;=&space;\frac{\left&space;|&space;A\cap&space;B&space;\right&space;|}{\left&space;|&space;A\cup&space;B&space;\right&space;|}" title="J(A,B) = \frac{\left | A\cap B \right |}{\left | A\cup B \right |}" /></a>

The equations show us, how Cosine and Jaccard Similarity will work. In Cosine Similarity, the smaller the angle and the greater the match between vectors. We can imagine this, as how close two objects. And then, For Jaccard, it compares members in two sets to see how many members are shared and which are distinct. The bigger size of the intersection, the higher score of Jaccard Similarity. So here it is, let say our customer choose ID Product 218:

![GitHub Logo](/images/cos11.png)

This is the top 3 Recommendation Products with Cosine Similarity Approach:

![GitHub Logo](/images/cos12.png)

And this is the top 3 Recommendation Products with Jaccard Similarity Approach:

![GitHub Logo](/images/cos13.png)

## Conclusion

In the recommendation system there is no better or worse system. But when we look from the results, I can say, they have a good results and the recommendations given are similar to the product chosen. For detail, can be seen in [this notebook](https://github.com/Stev-create/E-commerce-Product-Recommendations---Recommendation-System/blob/master/E-Commerce%20Product%20Recommendation.ipynb).






