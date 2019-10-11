# Fundamentals of Data Analysis -Project

## Introduction

Ìt is an established culture in the US is to tip with the standard being 15%.  One could argue that there is no need to conduct any analysis as it is an established practice and the relationship is definitive.  However that is short sighted as there are potentially behaviours that influence tip rate.  Is it possible to isolate the criteria that govern higher tip rate and increase pay for the server?  I am going to download the tips [6] dataset and utilise Python [1] packages, seaborn [5] and jupyter [4] to figure out if there are variables that influence tip %. 

#### Project Plan:
 -  Review and observe the dataset.  Visually observe if any variables look interesting or warrant further review either now or further on in the project.
    - Import the dataset
    - Use Pandas, Seaborn & Juypter to analyse statistics.
    - Regression: indepth discussion and analysis of whether there is a 
relationship between the total bill and tip amount.
    - Using jupyter [4], analyse the relationship between the variables within the dataset with reasonable investigation of  the relationship between the variables, with interesting relationships highlighted


### Review and Observance of dataset:
244 instances.  8 variables of different types:
3 numeric categories:  Total Bill, Tip & Party Size
4 Text catergories:   Sex, Smoker, Day & Time

Data appears clean.  Standard tip in the US is 15%.  Data from visual inspection of random lines appears to reflect the current trend.


### Import Dataset and libraries
The Tips dataset is downloaded from https://github.com/mwaskom/seaborn-data/blob/master/tips.csv.

Table 1:
Pandas describe() is utilised to summarise using statistics.  
Average bill is $19.68, average tip is $3 and average party size is 2.5. Tip % is 15.2%.
Volume of customers is key to higher tips as the bills are low.  Tips correlate to bill amount therefore tips are maximised with high customer throughput.  Overall this demonstrates that tip rate is representative of the perception of 15%.  However we need to dig a bit deeper to investigate if there are any underlying trends or dynamics that warrant further analysis.

Table 2:
Using pandas groupby function to slice the data, Thursday is the busiest day for lunch with 67 people served.  Only 7 customers had lunch on Friday.  No one was served lunch Saturday or Sunday meaning the server received no tips. 

Table 3:
Gender and Smoker status.  More males paid and the majority are non smokers.

## Is there a relationship between bill and tip amount?
This section reviews the factors that influence and determine tips.  
The question is why are there deviations regarding tips i.e. why do some people pay more or less.  The server in this dataset is the control therefore it is assumed that she treats all customers the same.  So on quieter days is she paid more as she can provide a better service and she does not have multiple customers to serve at the same time?  



Conclusion




References
 - [1] Python Software Foundation. Welcome to python.org.
https://www.python.org/.
 - [2] GMIT. Quality assurance framework.
https://www.gmit.ie/general/quality-assurance-framework.
 - [3] GitHub Guides. Mastering markdown.
https://guides.github.com/features/mastering-markdown/.
 - [4] Project Jupyter. Project jupyter.
https://jupyter.org/.
 - [5] Michael Waskom. seaborn.
https://seaborn.pydata.org/.
 - [6] Michael Waskom. Tips data set.
https://github.com/mwaskom/seaborn-data/blob/master/tips.csv.
