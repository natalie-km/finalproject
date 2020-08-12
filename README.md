# COVID High Risk Individuals, Hospital Beds and ICUs Across the United States
## By Natalie Keltner-McNeil

For my final project, I analyzed a [database](https://github.com/fivethirtyeight/data/tree/master/covid-geography) from Five Thirty Eight that shows the number of hospitals, ICU beds, and high risk individuals, or those likely to fall ill or die upon being infected with COVID-19, in micropolitan and metropolitan areas across the United States. The database combines [information](https://www.cdc.gov/brfss/smart/smart_2017.html) from the Center for Disease Control and Prevention and the Kaiser Family [Foundation](https://khn.org/news/as-coronavirus-spreads-widely-millions-of-older-americans-live-in-counties-with-no-icu-beds/#lookup). Individuals deemed high-risk included people over 65, those who had been diagnosed with chronic illnesses such as kidney disease, heart disease, and chronic bronchitis diabetes; those with asthma; the immunosuppressed; those with BMIs over 40; pregnant women; and those who smoke or vape every day.
The data was very clean, so I only changed the titles to clearer phrases once downloaded into Google Sheets. Then, I sorted most of the columns from A to Z or Z to A, to determine which regions had the most amount of individuals per ICU bed, the least hospitals, and the highest percent of at-risk people.
What I found interesting was that the regions which had the highest number of at risk individuals per hospital bed seemed to be mid-sized, semi-suburban towns and cities. This makes me think that age factored significantly into defining people as high risk.
I also found it interesting that the top regions with the fewest number of hospitals were predominantly in the south.
After sorting the data a little, I ran several pivot tables to interrogate it further. In the first, I created a list of the regions with the highest percent of high risk individuals per city or county. I narrowed the list by sorting conditionally to only include those regions with greater than 65 percent of people being high risk. Most of the regions were once again in the Midwest and South, with regions in Florida and South Carolina represented twice each.

![Screenshot of high risk regions pivot table](https://media.journalism.berkeley.edu/upload/2020/08/1597206102577feda.png)

I was curious which counties had the fewest ICU beds, and created a pivot table with all regions with less than 30 ICU beds. Google Sheets interpreted Provo-Orem, Utah as having 0 beds, when in actuality the data was missing. Thus, Kingsport-Bristol-Bristol, TN-VA had the least total ICU beds, with eight total. This is an area along the Virginia-Tennessee border, with several mid-sized cities and rural towns located along the Holston river. The semi-rural location could be a possible explainer for the lack of ICU beds in this region.

![Screen shot of ICU beds pivot table](https://media.journalism.berkeley.edu/upload/2020/08/1597206229ccb852e.png)

After running pivot tables, I constructed several charts. In the first, I created a [scatter](https://datawrapper.dwcdn.net/6awBQ/1/) plot charting the number of high risk individuals in the region versus the number of ICU beds. Besides seven outliers, there seemed to be a significant positive correlation between the number of high risk individuals and ICU beds per region. I am assuming the underlying variable is total population.

![Scatter plot](https://media.journalism.berkeley.edu/upload/2020/08/1597207086001f7db.png)

I then made a bar [chart](https://datawrapper.dwcdn.net/CHEkB/1/) from my pivot table on the regions with the highest percent of high risk people. 

![Bar chart showing regions with highest percent of high risk people](https://media.journalism.berkeley.edu/upload/2020/08/15972071953a65ac5.png)

Following that chart, I made a split bar [chart](https://datawrapper.dwcdn.net/AjNe1/1/) visually comparing the number of ICU beds per region to the number of hospitals per region. As expected, for the most part, ICU beds increased with the number of hospitals, besides for a few outlier regions, where there were only one or two ICU beds for a range between forty to eighty-three hospitals.

![Split Bar chart ICU beds and hospital beds per region](https://media.journalism.berkeley.edu/upload/2020/08/15972072854b48cc0.png)

In general, I was surprised at how many U.S regions had majority populations of high risk individuals. This provides further context into why total deaths from COVID are so high in the United States; we are an aging population and have many chronic illnesses. It would have been interesting to include race and income in this data, to see if hospital and ICU count correlates with either of those two social determinants of health.


