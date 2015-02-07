#Data Scientist's Toolbox - Week 1 (Overview)
##Overview

###What a data scientist do?

1. question
2. ideal data set
3. what can u access
4. obtain data
5. clean data
6. exploratory analysyis
7. stat prediction modeling
8. interpret
9. challenge
10. synthe / write
11. create reproducible code
12. distribute to 

##Getting help

###Some important R functions

*help function*
```
?rnorm
help.search("rnorm")
```
*get arguments*
```
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
	- RAW: original, hard to use, processing needed, processed once(maybe)
	- PROCESSED: ready, (merge, subsetting, transforming), may need standards, recordable
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

##Reproducible research
