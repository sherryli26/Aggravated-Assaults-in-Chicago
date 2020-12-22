### Xi Li
### December, 2020


What is the crime situation in different communities of Chicago and what are the factors behind the geospatial differences of crime rates? This project aims to let the audience know more about the crimes, aggravated assaults in particular, happening in communities of Chicago and the factors that are correlated with the discrepancy of crime rates. That not only enables people to have a better understanding of the crimes of Chicago, but also provides some insights for crime reduction.

### Data & Visualization Tools
The data used in this project is a combination of two datasets downloaded from Chicago government open portal: [Chicago Police Department Community Area Crime Data 1998-2009](https://chicagojustice.org/open-data/), and [The Community Information Dataset](https://data.cityofchicago.org/Public-Safety/Crimes-Map/dfnk-7re6). The crime dataset is from Chicago Justice Project. It provides information about the type and number of crimes occurred in different communities in Chicago from 1998 to 2009. The Community Information Dataset is from the public data of Illinois government.This data set is of 77 rows and 231 columns, containing very detailed information for 77 communities of the city of Chicago. Information not only includes general statistics like different kinds of population statistics(total, youth),the percentage of race, unemployment rate, but also covers more detailed aspects, for instance, commute methods, percentage of work type, etc. For this project, only variables concerned about the analysis are picked into the final dataset. In the final dataset, each observation is a community in one year, and the columns are the characteristics of that community and the number of crime happened there in that year.

Tableau, Plotly from Python and ggplot2 from R are used to create visualizations for this project.


## How Have Crime Rates Changed Overtime?
We can see from the plot that the numbers of all crimes in Chicago went down over time. Theft is the most common crime. Among all the violent crimes, aggravated assault has the highest occurrence rate. 


*Note: Double click on the crime rate legend on the right to hide a line. You can also select an area to zoom in. *

### What Are the Factors Behind Aggravated Assaults?
Aggravated assault is defined as “an unlawful attack by one person upon another for the purpose of inflicting severe or aggravated bodily injury” (FBI, 2017). In 2017, there are 810,825 cases of aggravated assault in the nation, which is 248.9 per 100,000 inhabitants. It is one of the most common type of crime in the city of Chicago. Researching on which factors are related with aggravated assaults helps police target crime-prone communities, enabling them to respond to crimes more efficiently, and enhance surveillance in these areas to prevent crime from happening. 

## Vacant/Underdeveloped Land
Below is a plot about communities in Chicago. The color filling in each area represents the percentage of vacant/underdeveloped land in that community. The deeper the color is, the higher the percentage is. The purple dots tell us about the crime rate of aggravated assaults. The bigger the circles are, the higher the crime rates are. We can see there is a correlation between the color and size of dots. In areas like the West Side, South Chicago and Englewood, there are high percentage of vacant land as well as aggravated assault rate.

<iframe seamless frameborder="0" src="https://public.tableau.com/views/underdevelopedlandandaggravatedassault/VacantLand?:language=zh-Hans&:display_count=y&publish=yes&:origin=viz_share_link&:showVizHome=no" width = '900' height = '600'></iframe> 

### Causal Relationship?
We already noticed the correlation between vacant land and aggravated assaults. However, to make policy suggestions to reduce crime, we also want to know whether there is a causal relationship between them. After doing a regression analysis controlling several variables including total population, employment rate, race, the percent of commercial and institutional land use, commute methods and main language used, I found that the percentage of vacant land is significant. That means the percentage of vacant land does have a causal effect on aggravated assaults. This graph demonstrates the effect.

![Image of causal effect](https://github.com/sherryli26/Aggravated-Assaults-in-Chicago/blob/main/images/causal_effect.PNG)

![Image of causal effect](https://github.com/sherryli26/Aggravated-Assaults-in-Chicago/images/causal_effect.png)

![Image of causal effect](/images/causal_effect.png)

### What Should We Do?

As we have the causal relationship here, we can start to clean the land to reduce crime. A lot of cases in the past already suggested cleaning vacant land can reduce crime effectively. [In Philadelphia, researchers analyzed 541 vacant lots that were randomly selected and assigned to either undergo inexpensive restoration or remain unchanged as a control site.](https://www.phillymag.com/news/2018/02/28/vacant-lots-crime-philly/) New grass, trash and debris removal and regrading are given to treated lots. Researches found that 18 months after restorations the treated lots had a lower crime rate. These cost-effective methods can be adopted in Chicago to clean vacant land too. After cleaning the land, we should install a split rail fence around it. This signals that although a lot is vacant, it isn’t abandoned. [According to “broken windows” philosophy of policing, minor crimes like littering and vandalism often invite more serious crime.](https://www.pewtrusts.org/en/research-and-analysis/blogs/stateline/2017/01/06/remaking-vacant-lots-to-cut-crime)A vacant lot can be sold to companies or organizations with a cheaper price after receiving basic cleaning. This helps reduce the government’s cost to maintain or develop the land. While cleaning the vacant land, the police should also target areas with higher percent of undeveloped land more, enhancing surveillance and patroling.

### Race
From this plot we can see that African American communities are distinctively more subject to aggravated assaults. The southern part of Chicago has been African American communities from decades ago, and that area has higher rate of aggravated assaults than its neighboring areas. Same for Austin on the north western side. 

<iframe seamless frameborder="0" src="https://public.tableau.com/views/underdevelopedlandandaggravatedassault/Race?:language=zh-Hans&:display_count=y&publish=yes&:origin=viz_share_link&:showVizHome=no" width = '900' height = '600'></iframe>

We should notice here that this is a correlation but not a causation. Also, there may be bias of the data behind this phenomenon. Crime data represents where the police go instead of where crime happens. The fact that the police target African American communities more may lead to the outcome that there are more crime cases in these communities. 

## Commute Methods
Another guess is that, does commute methods affect aggravated assault rate? Maybe the more people walk/bike to work, the more aggravated assaults happen? The plot rebuts this guess showing there are actually no correlation between them. 

<iframe seamless frameborder="0" src="https://public.tableau.com/views/underdevelopedlandandaggravatedassault/WalkingtoWork?:language=zh-Hans&:display_count=y&publish=yes&:origin=viz_share_link&:showVizHome=no" width = '900' height = '600'></iframe>


