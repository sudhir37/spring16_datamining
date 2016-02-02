EXAMPLE: EXPLORING INCOME AND EDUCATION DATASETS ON DATA.GOV
============================================================

OVERVIEW
--------

The US government (among many others around the world) has made a lot of data publicly available from the thousands of agencies that collect data either

-   as a consequence of the instruments and equipment they operate and run (e.g. weather data, seismic data, etc.),
-   as a function of the communities they serve (e.g. agriculture, legislation) or
-   because of the services they provide (e.g. transportation, labor statistics).

Many of these data are used to make day to day decisions that impact the everyday lives of people, but they also provide the inputs to many sophisticated models to make predictions about the future, for example, to predict the weather, or the amount of people flying through airports next year or the estimated number of unemployed workers next quarter and so on.

DATA
----

The IRS has an open dataset <https://www.irs.gov/uac/SOI-Tax-Stats-Individual-Income-Tax-Statistics-ZIP-Code-Data-(SOI)> that provides information about tax return data from 1998 to 2013 (with a few years missing in between). This data is organized around zip code and has Adjusted Gross Income (AGI), Wages and Salary data as well as dividend and interest information. It represents tens of thousands of data points.

RESEARCH QUESTIONS
------------------

We want to look for interesting patterns in the data which lead to a number of surface questions one could ask and go deeper later, for example:

-   What zip codes are the wealthiest by AGI, wages and salaries?
-   What are the correlations between the three? It would seem reasonable that wages and salaries are predictors of AGI? This may not be the case when dividend and interest income become factors.
-   Which zip codes have the highest dividend and interest income numbers? Are there any geographic surprises to the results?

These are just a series of tickler questions, as such an analysis could (and should) go much deeper …

Model building is the heart of the prediction side of data mining (and machine learning). Using a second dataset, we will explore another interesting question:

-   How do the educational data of zip codes or regions the zip codes cover correlate with the tax income data above? Is there a dataset that can be used to combine with the IRS data to determine relationships between primary and/or secondary schools and income? HINT: <https://catalog.data.gov/organization/ed-gov>.
- If there is a correlation, is there a way to be more precise about this relationship so we can explore it in depth to make predictions of the kind where we can determine how well an arbitrary zip code predicts educational outcomes?

MODELS AND ANALYSIS
-------------------

The models are described and the preliminary analyses were performed in a Jupyter Notebook found in our Github repo under analysis.



CODE AND APPLICATION
--------------------

The code is in Github and instructions on installation are in the README.md file.

PROJECT MANAGEMENT
------------------

Our team consists of two members, David B. and Greg P.; Greg did much of the front end work, while David did the back end. Front end work consisted of a web page that displayed visualizations and user interaction. Back end work consisted of an API that was created to provide data to the front end.

PROJECT DELIVERABLES AND CHECKPOINTS
====================================

| Checkpoint date | Expected Deliverable                                                          | Responsible team member(s) | Checkpoint results                                                                                                                  |
|-----------------|-------------------------------------------------------------------------------|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| 2/1/2016        | Exploratory data analysis of IRS data.                                        | David B., Greg P.          | Basic statistical information about the data; Jupyter notebook of results; cluster analysis of IRS data; code checked in to Github. |
| 2/15/2016       | Integration of school district data with IRS data.                            | Greg P.                    | Data testing completed.                                                                                                             |
| 2/29/2016       | Development of API for analysis reporting.                                    | David B.                   | API functionality complete; checked in to Github.                                                                                   |
|                 | Development of build and deployment script.  Development of API test harness. | Greg P.                    | Build scripts completed; test cases only at 30% of target (10 tests).                                                               |

(b) TEAM

| Team member | Roles and skills | Contributions |
|-------------|-------------------------|---------------------------------------------|
| Greg P. | Data analysis; testing | Data analysis; test harness; build scripts. |
| David B. | API development, Python | Web API, data analysis |
