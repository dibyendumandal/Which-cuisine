# Which cuisine?
*Can we predict the origin of a recipe (middle-easten, French, or Indian) from its ingredients?*

This is an end-to-end project involving data curated from [allrecipes.com](https://www.allrecipes.com/).  It applies standard classification algorithms (naive Bayes, logistic regression, and random forest) within the [Scikit-Learn](http://scikit-learn.org/) framework to predict the cuisine type of recipe from its ingredients. **Fun fact: All algorithms confuse some middle-eastern dishes to be Indian.**  

## Notebooks

As part of the project I analysed each of the cuisines first.  I downloaded the recipes from [Indian](https://www.allrecipes.com/recipes/233/world-cuisine/asian/indian/), [middle-eastern](https://www.allrecipes.com/recipes/235/world-cuisine/middle-eastern/), and [French](https://www.allrecipes.com/recipes/721/world-cuisine/european/french/) origin.  I analysed the typical ingredients present in these recipes in the following notebooks:

* [Indian](https://github.com/dibyendumandal/Which-cuisine/blob/master/Indian.ipynb)
* [Middle-eastern](https://github.com/dibyendumandal/Which-cuisine/blob/master/Middle_eastern.ipynb) 
* [French](https://github.com/dibyendumandal/Which-cuisine/blob/master/French.ipynb)

Next, I combined these analyses to predict the cuisine of a recipe from its ingredients. 

* [Prediction](https://github.com/dibyendumandal/Which-cuisine/blob/master/classification.ipynb)

**I accieved 80% accuracy in my prediction.**

## Data Wrangling

A particular challenge in the project was the presence of different forms for the the same word. For example, the word could be in plural form, in Indian language, in Arabic and so on.  Also, the recipes contained more than just the ingredients. For instance, they also 
mentioned the quantity for each ingredient(obviously!). I utilized the Python [natural lanluage toolkit](http://www.nltk.org/) to identify the nouns (ingredients) in the recipe.  The raw data are given in [recipe_data.csv](https://github.com/dibyendumandal/Which-cuisine/blob/master/recipe_data.csv).  Combined list of ingredients *(after much cleaning)* is given in [combined_ingredients.txt](https://github.com/dibyendumandal/Which-cuisine/blob/master/combined_ingredients.txt).  
