# Project 2 - Ames Housing Data and Kaggle Challenge (Work In Progress)

___
Problem Statement
---
`Situation`
* Alan Walker is a single , aspiring , working mid-profession currently living in Ames City. Like many of his peers in the working profession archetype, he is at a crossroad where he is looking to sell off his current house, so that he have sufficient capital to relocate to a bigger house to establish his new and impending growing family.

`Complication`
* Facing the financial challenge from their upcoming major life events (weddings , kids , new house, etc) , they often troubled over ways to optimise the selling price of their current house so as to lessen the finanicial burden arising from these events.

`Question (Problem Statement)`
* As a specialist in an established property and interior design team in Millenium Walk, how might we be able to use our housing prediction models to provide advise to house seller on which features to improve within their renovation spending budget , so that they are able to optimise their selling price between 5% to 10% from their current baseline Sale Price.

<a name = 'content_page'></a>
## Table of contents
* [Fast Fact on Ames City](#General-Info)
* [Datasets](#Data-Dictionary)
* [Regression Models](#Model)
* [Model's Result Summary](#Summary)
* [Key Observation](#Observation)
* [Application on Models on Client's Case Study](#Application)
* [Conclusion & Next Step](#Conclusion)

<a name = 'General-Info'></a>
## Fast Fact on Ames
___


<a name = 'Data-Dictionary'></a>
## Datasets and Data Dictionary
___
The data used for this project are from the following sources:

- DataSet :
- Data Dictionary:
- Training Dataset
- Test Dataset
- Additional Dataset for Feature Prediction

<a name = 'Model'></a>
## Regression Models & Results
___
* Linear Regression
* Lasso Regression
* Ridge Regression
* ElasticNet
* Random Forest Regression

|  | LR Score | Lasso Score | Ridge Score | Elastic Net | RandomForest Score |
|---:|---:|---:|---:|---:|---:|
| Training MAE | 0.076062 | 0.109778 | 0.076030 | 0.109778 | 0.036248 |
| Validation MAE | 0.078828 | 0.106090 | 0.077622 | 0.106090 | 0.075616 |
| Training RMSE | 0.104159 | 0.152725 | 0.104681 | 0.152725 | 0.052925 |
| Validation RMSE | 0.103474 | 0.147447 | 0.102304 | 0.147447 | 0.104506 |
| Training Model Score | 0.931745 | 0.853255 | 0.931058 | 0.853255 | 0.982378 |
| Validation Model Score | 0.924523 | 0.846741 | 0.926221 | 0.846741 | 0.923011 |

<a name = 'Summary'></a>
## Summary Intepretation on Model Results
___
* Include qualitative intepretation of these many decimal number


<a name = 'Observation'></a>
## Key Observation from Analysis
___

* To list down key features from

<a name = 'Observation'></a>
## Application on Models on Client's Case Study
___

* To list down how to use the model to predict
* what feature we used.
* how to interpret

<a name = 'Conclusion'></a>
## Conclusion & Next Step
___
[(back to top)](#content_page)

* Actual Qualitative Application
    1. In the `Section 6.0` Example , we were able to use our client baseline house condition, together with our Model to demostrate how variation of the feature affect the Sale Price. From `Section 6.2` , we had demostrate that if Alan (our client) were to renovate and improve his house condition from 5 to 7 , we predict he should be able to increase his Sale Price from `$270,000` to `$292,000` , a 8% potential increase.
    2. Overall , we were able to generate a model to advise our client what house features they could improve , and the qualitative correlation to the Sale Price. We could use our model to run on multiple features that had demostrated strong relation as demostrated in `Section 6.2` and `Section 6.3`
    3. We had also reached our model's target to be able to advise our client on what action to take on their house so that they are able to increase their selling price by 5% to 10%.

* Next Step
    * `While we are able to predict qualitatively , we should also take into account that to improve a house feature, renovation budget will be required. Whether that outweighs the increase of SalePrice is not covered in this studies and could be further studies together with interior design team.`



























