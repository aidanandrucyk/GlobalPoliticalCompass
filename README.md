# International Political Compass
Aidan M. Andrucyk | June 2020 | Google Colab (Jupyter Notebook) Environment
## For best user interaction, please use the [**Google Colab notebook**](https://colab.research.google.com/drive/1XhuR6I9JEl7EBBPQm05sesLyyV_8NyMp?usp=sharing) as many features including plotly graph interactivity are not available unless using a notebook. 
![CompassImage](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/International%20Political%20Compass.png)

**The final dataframe is contigent upon two major data sets: the Human Freedom Index and the Economic Freedom Index.**

### Human Freedom Index
The [**Human Freedom Index**](https://www.cato.org/human-freedom-index-new) captures the degree to which people are free to enjoy the major freedoms often referred to as civil liberties—freedom of speech, religion, association, and assembly— in the countries in the survey. In addition, it includes indicators on rule of law, crime and violence, freedom of movement, and legal discrimination against same-sex relationships. It also measures certain economic freedoms such as the freedom to trade or to use sound money.

### Economic Freedom Index
The [**Economic Freedom Index**](https://www.heritage.org/index/?version=318) tracks over two decades of the advancement in economic freedom, prosperity, and opportunity and promote these ideas in their homes, schools, and communities. The Index covers 12 freedoms – from property rights to financial freedom – in 186 countries. The measurement of economic freedom is based on 12 quantitative and qualitative factors, grouped into four broad categories, or pillars, of economic freedom:
* Rule of Law (property rights, government integrity, judicial effectiveness)
* Government Size (government spending, tax burden, fiscal health)
* Regulatory Efficiency (business freedom, labor freedom, monetary freedom)
* Open Markets (trade freedom, investment freedom, financial freedom)


### Description
* Visualized the relative economic and social ideologies of 159 countries on interactive scatter plots and choropleth world maps using plotly as well as distribution, categorical, correlation matrix, and regression plots using Seaborn.
* Utilized Pandas to clean, merge, and analyze Kaggle CSVs of indices on a Jupyter Notebook environment.

### Findings
* Personal freedom scores appear to be highest in first world countries and lowest in the Middle East and Northern Africa (MENA):<br/>
![EconomicWorldMapImage](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/personal_freedom_plotly_map.png)

* The standard deviation for each metric is less than the respective interquartile range (closest being economic freedom with .280689 > |(.185237-(-.179666))|, indicating few extremeties and a roughly symmetric spread.<br/>  
![describe_table](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/breakdown.png)

* There is a positive .63 pearson coefficient of correlation between the freedom and economic index scores, indicating a positive linear relationship of the freedom values.<br/>
* The following is a jointplot with a center scatter plot and side kernel density estimation plots:<br/>
![RegressionJointPlot](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/regressionjointplot.png)

* Most nations appear to either be in either extreme of Liberterian Right or Authoritarian Left (intuitively supports previous bullet):<br/>
![describe_ideology](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/ideology.png)

* The following is a kernel density estimation for each univariate catergory and a scatterplot for bivariate comparison (expansion upon previous bullet):<br/>
![Pairplot](https://github.com/aidanandrucyk/GlobalPoliticalCompass/blob/master/img/pairgrid.png)
