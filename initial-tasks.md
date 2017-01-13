## Overview
Rwanda has experienced substantial economic growth in the past decade.  However, chronic child malnutrition -- otherwise knowns as stunting -- remains high, with 37% of children under 5 being abnormally short for their age. The effects of stunting are long-term: stunted children have decreased cognitive development and poor physical development. Moreover, stunting has been associated with lower economic potential of countries. We’ve been working with USAID’s Rwanda office over the past year to help them identify where geographically stunting is highest, how stunting has changed over time, and what factors influence stunting.
In this project, you’ll process and analyze 2014/15 Rwanda Demographic and Health Survey Data to assess household-level factors associated with stunting in children under 60 months.


## 1. Get the data
Download the 2014/2015 Demographic and Health Surveys data from the [DHS website](http://dhsprogram.com/data/dataset/Rwanda_Standard-DHS_2015.cfm?flag=0):

* As a team, create an account to get access to the data (you can add 2 additional co-investigators).
* Download the all the survey data, including the geodata (rwge71fl.zip). If you're working in R, download all the files as Stata datasets (.dta).
* Import the data into R, python, or similar. If you’re using R, we recommend using package haven to import the data as a Stata (.dta) file using `read_dta`. This will maintain the variable and value labels to help you figure out what the data contain.

## 2. Read summaries of stunting in Rwanda
* [DHS Final Report](http://dhsprogram.com/publications/publication-FR316-DHS-Final-Reports.cfm) Focus on: 
  * Section 1 (INTRODUCTION)
  * Section 2 (HOUSEHOLD CHARACTERISTICS)
  * Section 11.1 (Nutritional Status of Children).

## 3. Figure out what's in the data
* [Explanation of what's inside each of the files](http://dhsprogram.com/data/Dataset-Types.cfm)
* Explore the data. Use variable labels. Look out for missing values (NA and coded values like '9', '996', '998', '999'). Note that all floating point (decimal) values are whole numbers.
* Skim through the [DHS recode manual](http://www.dhsprogram.com/pubs/pdf/DHSG4/Recode6_DHS_22March2013_DHSG4.pdf) and [recode map](http://www.dhsprogram.com/pubs/pdf/DHSG4/Recode6_Map_22March2013_DHSG4.pdf)
* Skim through the [DHS survey questionnaires](http://www.dhsprogram.com/publications/publication-DHSQ7-DHS-Questionnaires-and-Manuals.cfm)
* Glance at the [DHS forum](http://userforum.dhsprogram.com/) (user-submitted questions)

## 4. If there's time...
* Start to recreate the DHS's wealth index, which is the first principal component of a PCA on household-level assets.  Associated documentation:
[Initial academic paper on using PCA to make wealth indices] (http://vanneman.umd.edu/socy699J/FilmerP01.pdf)
[Tim's notes on how to create wealth indices]
[Overview page for how the DHS calculates wealth indices]
[PCA results from Rwanda (as .xlsx)]
[Paper talking about how wealth index is calculated]
[In-depth description of how wealth index is calculated in practice (variables, code)]

* Try your hand at creating your own wealth index. The DHS's is built for cross-country comparisons.  What variables would you add/subtract in the index?

## Goals for the first week
1. Understand how data is broken into models in the DHS.
* Understand how to merge data between models.
* Know where to look to figure out what are variables.
