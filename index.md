## Xi Li
## December, 2020


What is the crime situation in different communities of Chicago and what are the factors behind the geospatial differences of crime rate? This project aims to let the audience know more about the crimes, aggravated assaults in particular, happening in communities of Chicago and the factors that are correlated with the discrepancy of crime rates. That not only enables people to have a better understanding of the crimes of Chicago, but also provides some insights for crime reduction.

## Data & Visualization Tools
The data used in this project is a combination of two datasets downloaded from Chicago government open portal: [Chicago Police Department Community Area Crime Data 1998-2009](https://chicagojustice.org/open-data/), and [The Community Information Dataset](https://data.cityofchicago.org/Public-Safety/Crimes-Map/dfnk-7re6). The crime dataset is from Chicago Justice Project. It provides information about the type and number of crimes occurred in different communities in Chicago from 1998 to 2009. The Community Information Dataset is from the public data of Illinois government.This data set is of 77 rows and 231 columns, containing very detailed information for 77 communities of the city of Chicago. Information not only includes general statistics like different kinds of population statistics(total, youth),the percentage of race, unemployment rate, but also covers more detailed aspects, for instance, commute methods, percentage of work type, etc. For this project, only variables concerned about the analysis are picked into the final dataset. In the final dataset, each observation is a community in one year, and the columns are the characteristics of that community and the number of crime happened there in that year.

Tableau, Plotly from Python and ggplot2 from R are used to create visualizations for this project.


## How Have Crime Rates Changed Overtime?
We can see from the plot that the numbers of all crimes in Chicago went down over time. Theft is the most common crime. Among all the violent crimes, aggravated assault has the highest occurrence rate. 

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sherryli26/Crime-in-Chicago/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

## Pew
<a href="https://www.pewresearch.org/fact-tank/2020/11/20/facts-about-crime-in-the-u-s/ft_20-11-12_crimeintheus_5/"><img src="https://www.pewresearch.org/wp-content/uploads/2020/11/FT_20.11.12_CrimeInTheUS_5.png?w=474"></a>
