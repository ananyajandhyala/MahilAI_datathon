# data_analysis_proj
A project based on some basics of data science performed on a data set of of womens security in india.
# Task 1:
A dataset on crime against women is provided. Using this, analyze the data and find the
state/union territory which is the safest (relative lower crime rate).
Analyse by what percentage the crimes have been reduced in a particular state or against the
national average. Also, provide a suitable explanation for your analysis.
# Task 2:
A new column must be added to the existing dataset named ‘Safety index’. This column will
contain values based on how you interpret the safety of the district. For example, if the number
of abductions in a district is greater than 10, then decrease the safety index by 2%. Ideally, a
district with zero crime will have a safety index of 100%.
The participants can define the safety index with their own rule set. By coding (not manually)
update the dataset with the safety index for each district every year.

# OUR ANALYSIS:
We imported the required libraries such as pandas, numpy and matplotlib.pyplot to perform certain analysis on the given dataset. The first few lines of code try to extract the values of all the columns, conditioned on yearly basis. In order to calculate the mean of all crimes of a particular year we dropped the year value and used a built-in function to execute the above. The process was repeated till year 2014.
 A mathematical operation of simple percentage calculation was done in order to find the positive or negative growth rate from one year to the other. Based on the output, we can infer that the crime in the time period of 2011 to 2012 is about 5.9% , a significant increase was observed in the time frame of 2012 to 2013 peaking to 26.8% and a noticeable decrease in the years 2013 to 2014 holding the rate of 4.2%.
To help with data visualisation we aided it with a scatter plot and a pie chart.
Our code then explains on how we tried to add a new column called ‘safety index’, we first initialised it to hold 0 value. With the help of the join() function attached it to our modified dataset. This column describes the relative safety based on the ‘kidnapping and abduction’ values. For every district showing a value higher than 10 for the same reduces the safety index by 2%, (i.e., makes it 98 from the set point 100). The same was printed.
We then proceed to find the state/UT with the lowest crime rate in all categories it was to the union territory of Lakshadweep (it held the value 0 under each field).
We first group the data year wise for the respective state/UT and then we find mean. Then we find the index value of the row that corresponds to the least value within than category.
