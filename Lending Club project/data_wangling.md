          Data wrangling of Lending club data set 2015

1. Get unemployment rate in different zip code in US

Data resources:
a. https://www.kaggle.com/jayrav13/unemployment-by-county-us
b. https://www.gaslampmedia.com/download-zip-code-latitude-longitude-   city-state-county-csv/
c. https://github.com/liyepeng/Spring-Board-Data-Science-   Track/blob/master/Lending%20Club%20project/Three_state_unemploy.csv

Data cleaning:
Data a is about unemploymentrate in counties of USA in 2015. Cleaning job is to change states name to abbrievation, and add missing states unemployment information(3 states) from data c.

Data c is the information of counties and corrosponding zip codes. This data set contains 62 states among them there are associate states, millitary base. And the some county names are different from that in data a. Keeping 50 states information and making the counties' name match in both data a and data c are the majority of the cleaning work.

The last step is to combine data a and data b together. One county may has several zip code(XXX00 format) and one zip code may correspond with several county.  

2. Data wrangling for lending club data set

Data resources:https://www.lendingclub.com/info/download-data.action
a.Filling blank with 'NaN'. Because the tree based algorithmn doesn't matter the missing values I keep these values in original status.
b. Deleting blank columns, deleting post loan and hard ship varibles.
c. My target varible is loan_status and try to keep the varibles it help to make the decision for the loan.
d. Data format wrangling: get rid of '%', change the strings to lower case, check if there are duplicate records.
e. Data engineering: There are more than 100000 categories for emp_title varible. I choose top ten tiltes and create 10 dummy varibles so it can be used in EDA and model bulding.
f. Concating unemployment rate in different zip code file with lending club data set on zip code. My aim is to check if the unemployment rate has connection with loan status.
g. There are some outliers in the part of the numerical varibles. The way to deal with them is depending on what kind of machine learning algorithnms I plan to use.








