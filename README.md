# Titanic_Data_Analysis

This report looks at the Titanic data set to investigate the statistic of Titanic passenger and their socio-economical factors.
Descriptive statistics of the Titanic passenger

This dataset has 891 rows and 12 columns.  However there are considerable portion of the dataset that is missing. Only 183 rows have complete data for all the columns.

-Age:  First the data was cleaned fro m the data that do not an age value. The passengers’ age distribution is bimodal with median of 28. 
-Survival statistics: The survived statistics shows that 38.4% percent of passengers survived. The dataset have all the 891 survived values.

-Embarking locations: With regards of embarking locations; 72.4% belongs to S, 18.9 to C and 8.7% of passengers embarked at Q.  From all dataset 891, 889 row for embarking data   is available.

- Passengers’ sex: 0.65% of the passengers were male.

-> SOCIO-ECONOMIC of TITANIC POPULATION 

- Does socio-economic statue of adult unmarried women affect their survival rate?

The range of unmarried women is almost bimodal. The first modal is for teenage girls (age<18). However, a bigger portion of the is single women are their 20-40. It raises the question that if these women are among the top class of the society.

To find the marriage statues I used Pandas to separate passengers who have the word “Miss” in their names and are older than 18 years old. This group of unmarried women then grouped by their passenger class. Among 85 adult unmarried women 37(43.5%) where in class 1, 19(22.3%) in class 2 and 29(34.1%) in class 3. It shows that majority of young adult women who were single have the luxury to live in class one. However, a good portion of the women was in the cheapest class.  

The survival rate in unmarried girl is significantly depends on their class. Grouping by their class and survival, shows that class one only lost one passenger among 37 unmarried girls. Class 2, 2 passengers among 19 survived but in class 3, 17 among 29 of girls lost their life. 

- Did Titanic’s passengers’ room classes have subclasses? 

The classes of room in Titanic are 1,2,3. However, fair tickets of among within each are also different. So, It might be subclasses inside each class of rooms based on the location and luxurious auxiliaries of the room. 
First, pandas grouped the fares in ten dollars, and make a histogram. The histogram, unsurprisingly, shows three distinctive groups.  However, there are subclasses in each class 1,2, and 3. The presence of subclasses is especially renounced in the first class.
 
- Did upper class in Titanic passenger survived with higher rate?

Next, let us look at the effect of the class and ticket fare price on survival. If we group of the passenger by class, fare and survival. (the unknown value fare consider zero). We can look at the difference of survived and non-survived passengers in different socio-economic category. 

The last plot shows the different between frequencies of survived and not survived. The remarkable point in the analysis’s result is the affect of fare ticker price: subclasses inside each class. It shows that   more than class of the room the fare price was a key parameter to predict their life. For example, pricy 3rd class survived the same as low fare price of the first class.

 

-> LIMITATION OF ANALYSIS

•	The dataset is filled with missing values. The missing value in   data is omitted.
•	The statistical calculation is based on a sample of data and just provides a descriptive statistics, but statistical testing is needed to make a meaning full hypothesis.
•	There are other variables not included in the dataset such as the physical level of the rooms and their associated class; also the possibility of physical disabilities in passenger is another factor that can affect he survival likelihood. 


References:

-Stack over flow: how to count rows: (http://stackoverflow.com/questions/15943769/how-to-get-row-count-of-pandas-dataframe)


-Working with missing data:
(http://chrisalbon.com/python/pandas_missing_data.html)


