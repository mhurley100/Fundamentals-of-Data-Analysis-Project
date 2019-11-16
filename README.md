# Fundamentals of Data Analysis - 2019 Project

## Introduction

Ìt is an established culture in the US to tip.  Are there behaviours that influence tip rate?  Is it possible to isolate the criteria that govern higher tip rate and increase pay for the server? This project interrogates the tips [6] dataset and utilises Python [1] packages, seaborn [5] and jupyter [4] to analyse if variables presented influence tip %. If a strong correlation can be demonstrated, underlying relationships can be investigated for other relationships. 

#### Project Plan:
    - Import libraries
    - Import the dataset
    - Use Pandas[7], Seaborn[5] & Juypter[4] to describe statistically.
    - Regression: demonstrate correlation between the total bill and tip amount.
    - Using jupyter [4], analyse the relationship between the variables within the dataset with reasonable investigation of  the relationship between the variables, with interesting relationships highlighted.

### Libraries
Numpy, Pandas, Matplotlib, Seaborn & Csv libraries are imported.

### Import Dataset
The tips dataset from [6] Michael Waskom github repository is included to the repository.

### Description of Dataset:
Dataset is named 'tips' and run in Jupyter.  
Pandas[7] describe() is utilised to summarise using statistics.  
Average bill is $19.78, average tip is $3 with the minimum tip of $1 and max $10 and average party size is 2.5.   Overall this demonstrates that tip rate is representative of the perception of 15%.  However we need to dig a bit deeper to investigate if there are any underlying trends or dynamics that warrant further analysis.

### Regression of Dataset:
All groups paid a tip therefore a relationship does exist.  Using Pandas[7] groupby function to slice the data, Thursday is the busiest day for lunch with 61 groups served.  Only 7 groups had lunch on Friday.  No one was served lunch Saturday or Sunday meaning the server received no tips. This is very odd given that weekends should be the busiest time for restaurants.  It would seem that the restaurant is not attractive to young families or teenagers who would tend to go on outings at the weekend in particular at lunch.

Using Pandas[7] groupby function to slice the data by gender and smoker status.  More males paid and the majority are non smokers.
Barplot and histogram displayed.  Highest tip % is on Friday night. 
The histogram displays that tips are reasonably close to the average however there are outliers.

## Is there a relationship between bill and tip amount?
This section reviews the factors that influence and determine tips.  
The question is why are there deviations regarding tips i.e. why do some people pay more or less.  The server in this dataset is the control therefore it is assumed that she treats all customers the same.  So on quieter days is she paid more as she can provide a better service and she does not have multiple customers to serve at the same time? We are provided with 4 categories (smoker, sex, time and day). 
The average tip is $3, the min is $1 and max is $10.  

Target tip is calculated (15% of total bill). Minimum and maximum are established to allow for noise 5% upper and lower.

Conclusion

The majority of tips are in the range 10% to 20% which means that there is a correlation and customers do try to tip based on bill amount.
There is a strong relationship meaning underlying relationships can be investigated for other relationships. 


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
  - [8] Tripadvisor
 https://www.tripadvisor.ie/Travel-g191-s606/United-States:Tipping.And.Etiquette.html
  - [9] Bryant, P. G. and Smith, M (1995)
 Bryant, P. G. and Smith, M (1995) Practical Data Analysis: Case Studies in Business Statistics. Homewood, IL: Richard D. Irwin Publishing
  - [10] Dicook.public.iastate.edu
 https://dicook.public.iastate.edu/stat503/05/cs-tips2.pdf