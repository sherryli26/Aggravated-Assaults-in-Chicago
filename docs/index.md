### Xi Li
### December, 2020


What is the crime situation in different communities of Chicago and what are the factors behind the geospatial differences of crime rates? This project aims to let the audience know more about the crimes, aggravated assaults in particular, happening in communities of Chicago and the factors that are correlated with the discrepancy of crime rates. That not only enables people to have a better understanding of the crimes of Chicago, but also provides some insights for crime reduction.

### Data & Visualization Tools
The data used in this project is a combination of two datasets downloaded from Chicago government open portal: [Chicago Police Department Community Area Crime Data 1998-2009](https://chicagojustice.org/open-data/), and [The Community Information Dataset](https://data.cityofchicago.org/Public-Safety/Crimes-Map/dfnk-7re6). The crime dataset is from Chicago Justice Project. It provides information about the type and number of crimes occurred in different communities in Chicago from 1998 to 2009. The Community Information Dataset is from the public data of Illinois government.This data set is of 77 rows and 231 columns, containing very detailed information for 77 communities of the city of Chicago. Information not only includes general statistics like different kinds of population statistics(total, youth),the percentage of race, unemployment rate, but also covers more detailed aspects, for instance, commute methods, percentage of work type, etc. For this project, only variables concerned about the analysis are picked into the final dataset. In the final dataset, each observation is a community in one year, and the columns are the characteristics of that community and the number of crime happened there in that year.

Tableau, Plotly from Python and ggplot2 from R are used to create visualizations for this project.


## How Have Crime Rates Changed Overtime?
We can see from the plot that the numbers of all crimes in Chicago went down over time. Theft is the most common crime. Among all the violent crimes, aggravated assault has the highest occurrence rate. 

![Image of causal effect](https://github.com/sherryli26/Aggravated-Assaults-in-Chicago/blob/main/images/causal_effect.PNG)

![Image of causal effect](https://github.com/sherryli26/Aggravated-Assaults-in-Chicago/images/causal_effect.png)

![Image of causal effect](/images/causal_effect.PNG)



