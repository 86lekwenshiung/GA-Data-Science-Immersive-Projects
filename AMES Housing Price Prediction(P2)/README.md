# Project 2 - Ames Housing Data and Kaggle Challenge 
(ReadMe : Work In Progress)
(Main Readme : Done)
(Ppt : Work In Progress)

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
* [Credits and Resources](#Credits)

<a name = 'General-Info'></a>
## Fast Fact on Ames
[(back to top)](#content_page)


<a name = 'Data-Dictionary'></a>
## Datasets and Data Dictionary
[(back to top)](#content_page)
* The data used for this project are from the following sources:

- DataSet :[AMES Housing Dataset](https://www.kaggle.com/c/dsi-us-11-project-2-regression-challenge/data)
- Data Dictionary:[AMES Housing Set Dictionary](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)
- Training Dataset : 2051 Rows x 81 Features
- Test Dataset : 878 Rows x 80 Features
- Additional Test Dataset for Case Studies : 70 Rows x 80 Features , 25 Rows x 80 Features

<a name = 'Model'></a>
## Regression Models & Results
[(back to top)](#content_page)
* Linear Regression
* Lasso Regression
* Ridge Regression
* ElasticNet
* Random Forest Regression

|  | LR Score | Lasso Score | Ridge Score | Elastic Net | RandomForest Score |
|---|---|---|---|---|---|
| Training MAE | 0.075675 | 0.076120 | 0.075868 | 0.076094 | 0.035783 |
| Validation MAE | 0.075682 | 0.074083 | 0.074132 | 0.073673 | 0.075893 |
| Training RMSE | 0.104065 | 0.104905 | 0.104630 | 0.104878 | 0.052334 |
| Validation RMSE | 0.097977 | 0.095820 | 0.095426 | 0.095157 | 0.103696 |
| Training Model Score | 0.930951 | 0.929832 | 0.930199 | 0.929868 | 0.982537 |
| Validation Model Score | 0.933157 | 0.936069 | 0.936593 | 0.936950 | 0.925127 |

<a name = 'Summary'></a>
## Summary Intepretation on Model Results
[(back to top)](#content_page)
* 4 of 5 models performed relatively well with respect to the Validation Dataset , generally not overfitting (Except for RF).
* Validation RMSE in the range of 0.093 - 0.104. This means that on average, the predicted value is 9.74% - 10.9% away from my actual results.
* On Average, the predicted value will be $17810 to $18840 away from the actual results , depending on the model used.


<a name = 'Observation'></a>
## Key Observation from Analysis
[(back to top)](#content_page)

* To list down key features from

<a name = 'Observation'></a>
## Application on Models on Client's Case Study
[(back to top)](#content_page)

1. We establish the baseline score for our client model, in this example , the key features as show:
|  | LR Score | Lasso Score | Ridge Score | Elastic Net | RandomForest Score |
|---|---|---|---|---|---|
| Training MAE | 0.075675 | 0.076120 | 0.075868 | 0.076094 | 0.035783 |
| Validation MAE | 0.075682 | 0.074083 | 0.074132 | 0.073673 | 0.075893 |
| Training RMSE | 0.104065 | 0.104905 | 0.104630 | 0.104878 | 0.052334 |
| Validation RMSE | 0.097977 | 0.095820 | 0.095426 | 0.095157 | 0.103696 |
| Training Model Score | 0.930951 | 0.929832 | 0.930199 | 0.929868 | 0.982537 |
| Validation Model Score | 0.933157 | 0.936069 | 0.936593 | 0.936950 | 0.925127 |
2. Using Our Model , we are able to demostrate the qualitative impact of improving a feature score ; in this example , the house and garage condition
3. Example of Qualitatative Impact:
![](https://github.com/86lekwenshiung/GA-Data-Science-Immersive-Projects/AMES Housing Price Prediction(P2)/images/House_cond.png)

<a name = 'Conclusion'></a>
## Conclusion & Next Step
[(back to top)](#content_page)

* Actual Qualitative Application
    1. In the `Section 6.0` Example , we were able to use our client baseline house condition, together with our Model to demostrate how variation of the feature affect the Sale Price. From `Section 6.2` , we had demostrate that if Alan (our client) were to renovate and improve his house condition from 5 to 7 , we predict he should be able to increase his Sale Price from `$270,000` to `$292,000` , a 8% potential increase.
    2. Overall , we were able to generate a model to advise our client what house features they could improve , and the qualitative correlation to the Sale Price. We could use our model to run on multiple features that had demostrated strong relation as demostrated in `Section 6.2` and `Section 6.3`
    3. We had also reached our model's target to be able to advise our client on what action to take on their house so that they are able to increase their selling price by 5% to 10%.

* Next Step
    * `While we are able to predict qualitatively , we should also take into account that to improve a house feature, renovation budget will be required. Whether that outweighs the increase of SalePrice is not covered in this studies and could be further studies together with interior design team.`

<a name = 'Credits'></a>
## Credits and Resources
[(back to top)](#content_page)
























