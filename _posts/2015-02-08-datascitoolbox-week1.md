---
title: Data Scientist's Toolbox - Week 1
layout: post
---

##Overview

###What a data scientist do?

1. find the right question
2. figure out the ideal data set
3. figure out what can be accessed
4. obtain data
5. clean data
6. perform exploratory analyses
7. develop statistical and prediction models
8. interpret results
9. challenge results
10. synthesize / write results
11. create reproducible code
12. distribute findings to others

##Getting help

###Some important R functions

*help function*

```R
?rnorm
help.search("rnorm")
```

*get arguments*

```R
args("rnorm")
```

### R Questions

1. How to reproduce the problem
2. What your expect
3. What you see
4. Version of R (or package)
5. OS?

### Data analysis questions
1. Question to solve?
2. Steps/tools?
3. What you expect
4. What you see
5. Other solutions?

##Finding Answers

![data science venn](http://static1.squarespace.com/static/5150aec6e4b0e340ec52710a/t/51525c33e4b0b3e0d10f77ab/1364352052403/Data_Science_VD.png?format=750w "drew conway")

source: [the-data-science-venn-diagram](http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram)

scattered information >> hacking skills needed
### Skills
 - find andswers 
 - Know where to look
 - Unintimidated by new stuff
 - Unafraid to say they don't know
 - *Polite but relentless*

##R Programming Overview

### reading a text file

```R
con <-url("uri")
x <- readLines(con)
>head(x)
```

### apply function to all elements

```R
lapply(list, function, args) 
```

*looping internally in C code*

##Getting and Cleaning Data

- raw vs tidy data
	- **RAW:** original, hard to use, processing needed, processed once(maybe)
	- **PROCESSED:** ready, (merge, subsetting, transforming), may need standards, recordable
- download 
- reading: XLS, JSON, MySQL, ...
	- listing DBs

	```R
	db <-  dbConnect(MySQL(), user="me", host="127.0.0.1")
	result <- dbGetQuery(db, "show databases;")
	dbDisconnect(db)
	result
	```

- merging

	```R
	merged <- merge(review, soulutions, by.x = "sol_id", by.y = "id", all=TRUE)
	head(merged[,1:6], 3)
	reviews[1, 1:6]
	```

- reshaping
- summarizing
- finding/replacing
- data resources



##Exploraratory analysis

1. Analytic Graphics principles
	1. show comparisons
	2. show causality, mechanism, explanation
	3. show multivariate data
	4. integrate multiple modes of evidence
	5. describe and document the evidence
	6. content is king
2. Exploratory graphs
3. Plotting systems in R
4. Hierarchical clustering
5. K-Means clustering
6. Dimension reduction

## Reproducible research

1. Data analysis: structure
	- *look up*
	- Files:
		- Data: raw and processed
		- Figures: exploratory and final
		- R code: raw and final scripts, R markdown 
		- Text: Readme, text of analysis

2. Data analysis: organizing
3. Markdown
4. LaTeX
5. R Markdown
6. Evidence-based data analysis
7. RPubs


## Statistical inference

1. Basic probability
2. Likelihood
3. Common distributions
	- normal, gaussian, standard...
4. Asymptotics
5. Confidence intervals
6. Hypothesis tests
7. Power
8. Bootstrapping
9. Non-parametric tests
10. Basic bayesian stats

## Regression Models

1. Linear regression
2. Multiple regression
3. Confounding
4. Residuals and diagnostics
5. Prediction using linear models
6. Model misspecification
7. Scatterplot smoothing/splines
8. Machine learning via regression
9. Resampling inference in regression, bootstrapping, permutation tests
10. Weighted regression
11. Mixed models (random intercepts)

## Practical Machine Learning

1. Prediction Study Desing
2. Type Of Errors
3. Cross Validation
4. The Caret Package
5. Plotting For Prediction
6. Preprocessing
7. Predicting With Regression
8. Predicting With Trees
9. Boosting
	- AdaBoost
10. Bagging
11. Model Blending
12. Forecasting

- sensitivity and specificity
- correlated predictors

## Building Data Products

1. R packages
	- devtools
	- roxygen
	- testthat
2. rCharts
3. Slidify
4. Shiny

## Installing R



## Installing RStudio

