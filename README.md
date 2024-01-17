# Basic Analysis with Excel

On the first challenge, we're helping Louise visualize data to get a first look and highlight some possible niche in the market.

## Outcomes of theatrical productions

### Identify performance of theater plays based on launch date and funding goals

By use of basic excel tools, it could be seen in a graphic content the trend of any sorted data. Though analysis could be made on a greater scale, the focus was made on a particular matter, success relative to launch date and monetary goals. Data will be analyzed to represent the outcomes of theatrical productions plays.

---

## Analysis and Challenges

As data comes in raw, even though it's organized, there should be made some kind of display arrangement to interpret it.

### Analysis of Outcomes Based on Launch Date
Filtering and sorting data will be the fisrt step. It can be a challenge as data is not ready to use, it has to be done a conversion of the dates from Unix timestamps (using a simple conversion formula that takes into consideration the seconds, minutes and hours of a day from 1/1/1970 as reference), and the "=YEAR()" excel function to extract the year at the time of opening, also separating the Parent categories and subcategories (using the 'Text to columns' tool on the Data tab) will be useful to sort data through parent category 'Theater' or subcategory 'plays'.

By creating a pivot table, taking as filters reference parent category 'Theater' and 'years' we can compare successful, failed and canceled outcomes in a calendar year. This relation could be appreciated in the following chart.

![Theater_Outcomes_vs_Launch.png](/Resources/Theater_Outcomes_vs_Launch.png)

It can be seen from this chart that there are more succesful plays than failed ones, failed plays follow similar trends throughout the months of the years and it can be seen that there are more number of plays in some months, and as a result there are more chances of succeed as seen in peak on May. 

Besides the sorting of the data to be readable and useful, another challenge using data could be selecting the appropiate information to take into account to create relationships and showcase results. In this case, filtering through plays on a pivot chart over the years, led us to collect useful information about the outcomes compared to analyze every individual year (which leads to inconclusive results). 

### Analysis of Outcomes Based on Goals
This time, a tabular table was created based in our Kickstarter data to count for ranges of amount on initial monetary goals, using subcategory 'plays' as filtering reference and by implementing the "=COUNTIFS()" excel tool. Likewise, operations in the outcomes column to filter and extract the information needed, the function "=SUM()" to group the results and evaluate percentages, made with a basic mathematical calculation (Outcome/SUM * 100) inside  "=IFERROR()" function, to prevent errors from data with zero values. A visual representation of percentage of success, failure and canceled plays is displayed in the following line chart. 

![Outcomes_vs_Goals](/Resources/Outcomes_vs_Goals.png)

One visible trend in this chart is that, higher funding goals for plays tend to have a negative effect on how well it performed. Someone could easily point that in the range of 35000 to 49999 there were some succesful plays, but that is not an indicator that correlates to data accurately, as successful plays tendency is seen to decrease and the amount of plays in that range is very small (compared to lesser funding goals).

Possible challenges could be present if there was a more specific question that requires calculations and use of more complex formulas to work with or with an increased quantity of data which gives more room for error or outlier data points. 

--- 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
 
 There are more successful theater productions at any time of the year.
 
 May is a great month for theater productions.

- What can you conclude about the Outcomes based on Goals?
 
 Higher funding goals plays often results in failed outcomes.
 
 There are more chances of success with funding goals set less than $20,000.

- What are some limitations of this dataset?

Limitations could be the adittional steps made to clean the data to use for the analysis. With this done, there's a lot of different categories for the information supplied, so whenever theres any specific topic to address, some of the data falls off the analysis and shortens our dataset. 

- What are some other possible tables and/or graphs that we could create?

With the Outcome column, it can also be possible to check another category that wasn't taking into consideration, like 'Music'. While doing the same analysis of the outcome one can see that it has a more succssesful rate than Theater. 

![Music_Outcomes_vs_LaunchDate.png](/Resources/Music_Outcomes_vs_LaunchDate.png)

As it can be seen, there are fewer failed and canceled outcomes. Digging deeper into subcategories it can be seen the succesful ones by the genre of 'rock', 'pop', 'electronic music' and 'metal', to name some.


