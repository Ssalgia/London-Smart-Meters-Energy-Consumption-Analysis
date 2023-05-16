# London-Smart-Meters-Energy-Consumption-Analysis

This Project was completed in the DataBricks using PySpark, MLSpark and Spark SQL. 

### OBJECTIVE :
The goal of this analysis is to understand energy consumption pattern in London. The dataset consisted of 5,566 London households and their energy consumption between November 2011 and February 2014. The readings for each household were taken every half hour. Households in UK have been allocated to CACI ACORN(Classification of Residential Neighborhoods) categories, which is a geo-demographic segmentation of UK's population. There are 6 such categories. Each of these 6 categories are further divided into groups, making a total of 18 groups. More information about ACORN groups can be found here.

### OVERVIEW :
UK's energy tariff plans are categorized into two groups: Dynamic Time of Use and Standard. The Dynamic Time of Use plan is set up in such a way that each household is informed in advance of the specific times when their electricity tariff would be higher or lower than normal price– High (67.20p/kWh), Low (3.99p/kWh) or normal (11.76p/kWh). The Standard plan has a constant flat rate(14.228p/kWh) throughout the day.

This dataset was used to understand energy consumption patterns across different ACORN groups. Initial analysis consisted of understanding the different ACORN groups and the difference between them. The next steps of analysis consisted of a deep dive into the dataset which contains the records of household energy consumption (monitored every half hour) to try to establish different consumption patterns based on tariff plans and the ACORN groups. Analysis of weather impacts on energy consumption across groups was also conducted. The resulting output comprised of visualizations of various parameters which exhibit energy consumption trends within and across ACORN groups.

Different tariff plans were introduced in UK to reduce overall energy consumption. Dynamic Time of Use (DToU) plan provided users with different tariff rates(high/normal/low prices)so that subscribers could effectively plan their energy usage, thereby, reducing their overall consumption. Displayed in the chart above is the average energy consumption by different tariff plan subcribers for each ACORN classification over a span of roughly 2 years. It was seen that mean energy consumption for DToU subcribers were lower than the standard tariff plan subscribers in the case of Affluent and Adversity ACORN groups whereas for the comfortable ACORN group it was exactly opposite.

Energy usage was very high during evening hours, less during day time and mean energy usage dips down to the lowest during late night hours. This pattern remains same irrespective of their tariff rates (high, normal, low). Also, it is seen that less energy is consumed when high rates are charged.

Energy consumption was high from December to March. The average temperature for the same period was below 5°C and thus, this explains higher energy consumption during this period as heating systems would have been used extensively. Thus, temperature change plays a major role in energy consumption irrespective of different ACORN groups.

#### Summary
To summarize, energy consumption varies depends upon:

Temperature
Applied tariff rates
Different tariff plans(Std./DToU)
ACORN classification
Dependencies:
Python Packages used:
pandas
numpy
matplotlib
seaborn
datetime
plotly
calendar
### Datasets used:
https://www.kaggle.com/jeanmidev/smart-meters-in-london

https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households


