# Fundamentals of Data Analysis - 2019 Project

## Introduction

Ìt is an established culture in the US to tip with the standard being 15%.  Are there behaviours that influence tip rate?  Is it possible to isolate the criteria that govern higher tip rate and increase pay for the server?  I am going to interrogate the tips [6] dataset and utilise Python [1] packages, seaborn [5] and jupyter [4] to figure out if there are variables that influence tip %. 

#### Project Plan:
 -  Review and observe the dataset.  Visually observe if any variables look interesting or warrant further review either now or further on in the project.
    - Import the tips[6] dataset
    - Use Pandas[7], Seaborn[5] & Juypter[4] to analyse statistically.
    - Regression: indepth discussion and analysis of whether there is a 
relationship between the total bill and tip amount.
    - Using jupyter [4], analyse the relationship between the variables within the dataset with reasonable investigation of  the relationship between the variables, with interesting relationships highlighted.


### Visual Review and Observations of dataset:
244 instances.  8 variables of different types:
3 numeric categories:  
    - Total Bill
    - Tip
    - Party Size
4 Text categories:
    - Sex
    - Smoker
    - Day
    - Time

Data appears clean.  Data from visual inspection of random lines appears to reflect the current trend with some outliers.  Tip % needs to be added.  It is also difficult to tell whether the tip is within range.    

### Import Dataset and libraries
The tips [6] dataset from github is copied to the repository, imported and initial tables generated using Pandas[7].  Tip % is added as it is not included in the dataset.

Table 1:
Pandas[7] describe() is utilised to summarise using statistics.  
Average bill is $19.68, average tip is $3 with the minimum tip of $1 and max $10 and average party size is 2.5. Tip % is 15.2%.  The restaurant is not expensive therefore the tips are going to be low therefore volume of customers is needed.  Overall this demonstrates that tip rate is representative of the perception of 15%.  However we need to dig a bit deeper to investigate if there are any underlying trends or dynamics that warrant further analysis.

Table 2:
Using Pandas[7] groupby function to slice the data, Thursday is the busiest day for lunch with 61 people served.  Only 7 customers had lunch on Friday.  No one was served lunch Saturday or Sunday meaning the server received no tips. This is very odd given that weekends should be the busiest time for restaurants.  It would seem that the restaurant is not attractive to young families or teenagers who would tend to go on outings at the weekend in particular at lunch.

Table 3:
Using Pandas[7] groupby function to slice the data by gender and smoker status.  More males paid and the majority are non smokers.
Perhaps having a smoking section is eliminating a potential target market i.e. families and teenagers?

Barplot and histogram displayed.  Highest tip % is on Friday night. 
The histogram displays that tips are reasonably close to the average however there are outliers.

## Is there a relationship between bill and tip amount?
This section reviews the factors that influence and determine tips.  
The question is why are there deviations regarding tips i.e. why do some people pay more or less.  The server in this dataset is the control therefore it is assumed that she treats all customers the same.  So on quieter days is she paid more as she can provide a better service and she does not have multiple customers to serve at the same time? We are provided with 4 categories (smoker, sex, time and day). 
The average tip is $3, the min is $1 and max is $10.  

Target tip is calculated (15% of total bill). Minimum and maximum are established to allow for noise 5% upper and lower.

Conclusion

The majority of tips are in the range 10% to 20% which means that there is a correlation and customers do try to tip based on bill amount.

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
 - [7] Pandas Data Analysis library
 https://pandas.pydata.org.