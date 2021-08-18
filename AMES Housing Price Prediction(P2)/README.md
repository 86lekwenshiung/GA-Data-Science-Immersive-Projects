# Project 2 - Ames Housing Data and Kaggle Challenge
(ReadMe : Work In Progress)
(Main Readme : Done)
(Ppt : Work In Progress)

___
Problem Statement
---
`Situation and Complication`
* Alan Walker is a single , aspiring , working mid-profession currently living in Ames City. Like many of his peers in the working profession archetype, he is at a crossroad where he is looking to sell off his current house, so that he have sufficient capital to relocate to a bigger house to establish his new and impending growing family.
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
- Test Dataset for Business Case : 70 Rows x 80 Features , 25 Rows x 80 Features

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
## What those number tell us?
[(back to top)](#content_page)
* 4 of 5 models performed relatively well with respect to the Validation Dataset , generally not overfitting (Except for RF).
* Validation RMSE in the range of 0.093 - 0.104. This means that on average, the predicted value is 9.74% - 10.9% away from my actual results.
* On Average, the predicted value will be $17810 to $18840 away from the actual results , depending on the model used.


<a name = 'Observation'></a>
## Key Observation from Models?
[(back to top)](#content_page)

* To list down key features from

<a name = 'Observation'></a>
## Application on Models on Client's Business Case
[(back to top)](#content_page)

1. We establish the baseline score for our client model, in this example , the key features as show:

| Feature (Curent State of House) | Description |
|---|---|
| Neighborhood | NridgHT |
| House Style  | 2 Story |
| Living Area  | 1,904 SF |
| Functional  | Typical |
| Air Con  | Yes |
| Current House Cond | 5 |
| Current House QC | 8 |
| Current Garage Cond | Typical Average |
| Current Garage QC | Typical Average |

2. Using Our Model , we are able to demonstrate the qualitative impact of improving a feature score ; in this example , the house and garage condition
3. Example of Qualitatative Impact:

<p align = 'center'>
    <img src = 'images/House_cond.png' height="47%" width="47%"> 
    <img src = 'images/Garage_cond.png' height="50%" width="50%">
</p>

<a name = 'Conclusion'></a>
## Conclusion & Next Step
[(back to top)](#content_page)


* While we are able to predict qualitatively , we should also take into account that to improve a house feature, renovation budget will be required. Whether that outweighs the increase of SalePrice is not covered in this studies and could be further studies together with interior design team.

<a name = 'Credits'></a>
## Credits and Resources
[(back to top)](#content_page)
