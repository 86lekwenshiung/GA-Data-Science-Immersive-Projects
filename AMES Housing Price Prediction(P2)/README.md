# Project 2 - Ames Housing Data and Kaggle Challenge

___
Problem Statement
---
`Situation`
* Alan Walker is a single , aspiring , working mid-profession currently living in Ames City. Like many of his peers in the working profession archetype, he is at a crossroad where he is looking to sell off his current house, so that he have sufficient capital to relocate to a bigger house to establish his new and impending growing family.

`Complication`
* Facing the financial challenge from their upcoming major life events (weddings , kids , new house, etc) , they often troubled over ways to optimise the selling price of their current house so as to lessen the finanicial burden arising from these events.

`Question (Problem Statement)`
* As a specialist in an established property and interior design team in Millenium Walk, how might we be able to use our housing prediction models to provide advise to house seller on which features to improve within their renovation spending budget , so that they are able to optimise their selling price between 5% to 10% from their current baseline Sale Price.


## Table of contents
* [General info](#general-info)
* [Technologies](#3.0-Data-Dictionary)
* [Setup](#setup)

## General info
This project is simple Lorem ipsum dolor generator.

___
## 2.0 Datasets and Additional resources
---
The data used for this project are from the following sources:

- 2017 to 2019 SAT Datasets by States
- 2017 to 2018 ACT Datasets by States
- https://www.census.gov/topics/income-poverty.html
- https://worldpopulationreview.com/state-rankings/average-income-by-state
- https://www.census.gov/library/visualizations/interactive/2019-median-household-income.html
- https://fred.stlouisfed.org/release/tables?eid=259515&rid=249#
- https://www.collegeraptor.com/getting-in/articles/act-sat/states-act-sat-given-free/
- https://mindfish.com/which-states-require-the-sat/
- https://www.statology.org/what-is-a-strong-correlation/

___
## 3.0 Data Dictionary
---
|Feature|Type|Dataset|Description|
|---|---|---|---|
|State|index|SAT/ACT|State names for 50 states in the US, plus District of Columbia|
|sat_pr_2017|float|SAT|State-wide participation rate (%) in 2017| 
|sat_erbw_2017|int|SAT|State mean score for Evidence-Based Reading and Writing (ERW) in 2017|
|sat_math_2017|int|SAT|State mean score for Math in 2017|
|sat_total_2017|int|SAT|State mean total (combined score for ERW and Math) in 2018|
|sat_pr_2018|float|SAT|State-wide participation rate (%) in 2018| 
|sat_erbw_2018|int|SAT|State mean score for Evidence-Based Reading and Writing (ERW) in 2018|
|sat_math_2018|int|SAT|State mean score for Math in 2018|
|sat_total_2018|int|SAT|State mean total (combined score for ERBW and Math) in 2018|
|sat_pr_2019|float|SAT|State-wide participation rate (%) in 2019| 
|sat_erbw_2019|int|SAT|State mean score for Evidence-Based Reading and Writing (ERBW) in 2019|
|sat_math_2019|int|SAT|State mean score for Math in 2019|
|sat_total_2019|int|SAT|State mean total (combined score for ERBW and Math) in 2019|
||
|act_pr_2017|float|ACT|State-wide participation rate (%) in 2017| 
|act_total_2017|float|ACT|State mean composite score (average score for English, Math, Reading, and Science) in 2017|
|act_pr_2018|float|ACT|State-wide participation rate (%) in 2018| 
|act_total_2018|float|ACT|State mean composite score (average score for English, Math, Reading, and Science) in 2018|
|act_pr_2019|float|ACT|State-wide participation rate (%) in 2019| 
|act_total_2019|float|ACT|State mean composite score (average score for English, Math, Reading, and Science) in 2019|
||
|2019 Household Median Income|float|State|2019 Median Household Income by US States| 
|2019 Household Ranking|float|State|2019 Median Household Income Ranking by US States. No.1 has highest median household income|
|2019 Gini Coeff|float|State|2019 Gini Coefficient by US States| 
|2019 Gini Ranking|float|State|2019 Gini Coeff Ranking by US States. No.1 has lowest Gini Coeff.|
|2019 Poverty Rate|float|State|2019 Poverty Rate in % by US States| 

___
## 4.0 General Summary of Findings
---
**Participation Rate (PR)**
* 100% SAT participation rates for 3 states and 100% ACT participation rates for 13 states from 2017 : 2019. Most of these states are inside the mandatory SAT and ACT rules respectively.
* General trend that states that have high PR in one test will have a lower PR in another test. For example, a state that has high PR in SAT will have low PR in ACT. This trend make sense as well, since usually students are only required to take either or. **See section 3.2 for the supporting graph visualisation**
* 3 States (Florida , Georgia , Hawaii) had >50% participation rate for both test in 2017. 5 States (Florida , Georgia , Hawaii , North and South Carolina) achieved that in 2018. Georgia fall below the 50% mark for ACT in 2019
* Colorado appear to have a change in mandatory from ACT in 2017 to SAT in 2018
___

**Score**
* States are usually specialised in scoring well in one of the test ; There is no State that score well in both SAT ands ACT. **See section 3.1 scatter plot for suppporting graph visualisation**
* New Hampshire , Massachusetts , Connecticut have consistently top the ACT score from 2017 to 2019
* South Carolina , Mississippi , Nevada have consistently bottom the ACT score from 2017 to 2019
___

**Score and Participation Rate (PR) Relationship**
* PR have an inverse relation with Score. Lower Participation rate in a test , generally have a better score. This could be due to the possible reasoning that these participants are taking additional tests as secondary supplement, and since they are competetive in personal nature, they tend to work harder and score better. Furthuermore, there will also be lesser non-motivated people to dilute the score. **See Section 3.3 for the supporting graph visualisation**
___

## 5.0 Specific Finding and recommendation with relation to Median HouseHold Income
___

By doing a systematic zoom-in on the effect of household income on the test score, we summarised our key insights as below :

### Key Insights
1. Base on correlation heatmap , poverty rate and household median income has a moderately strong impact on ACT score (~0.6). Since Poverty Rate and household income strong correlation with each other, we will take 1 of these 2 to further study into the score and PR.
2. It is observed that Household Income had a relatively strong correlation with the ACT score , but not the SAT score.
3. Consider all State , based on the bottom 12 median income state, only 1/12 state score above the 25% for ACT while 9/12 state score above the 25% percentile for SAT. Consider only non-mandatory state , based on the bottom 5 median income state, only 4/5 state score above the 25% for ACT while 1/5 state score above the 25% percentile for SAT.
4. Out of the 12 least median household income state , 9 out of 12 states had high PR in ACT.


### Recommendation
Based on limited resources , the government should focus on fininicial aid to lower median household in Mississippi , Arkansas , Louisiana , Alabama, Kentucky , Oklahoma aiming to take ACT so that the state can aim to increase their score toward the 25% score percentile by 2021
