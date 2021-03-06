# Management for COVID19 Pandemic Through Python Data Analysis
COVID19 is a newly discovered infectious disease that's spreading illness, fear, and uncertainty in all sectors of society. 
It's a challenge for individuals, businesses, organizations, and governments which makes it particularly crucial for data analysis on existing and updating information on the virus characteristis, age/sex groups that are more at risk,resources available, and effects on important institutions. 
Effective data management can help minimize these the effects and help decision-makers better allocate resources and attention given the trends. 

**Business Question**
Based on demographics and hospital availability, which FIPS counties are the most vulnerable or at risk during COVID19?

It's important to address this to allow policymakers in each region to implement practices like social distancing and businesses to prepare workers and supplies to support these weaker areas. 

**Data Question**
What metrics and data do we have to monitor healthcare resources and COVID19 conditions in the given counties?

## Data Interpretation
![Unknown-2](https://user-images.githubusercontent.com/60996310/80255350-ba542500-864a-11ea-8ddc-5675a2da75eb.png)


The **bar chart** conveys 20 counties with the highest populations with Los Angeles County, California taking a significant lead at 10.1M; its high number of people suggests that the county is most at risk for virus transmission, but zoning into population density and certain characteristics (i.e. percent of people over the age of 60) reveal that although certain counties are less populated, they may be more at risk and thus require more attention. 

![Unknown-3](https://user-images.githubusercontent.com/60996310/80255429-deb00180-864a-11ea-8b7d-6b50a3f9d7ee.png)


As seen in the **scatter chart**, there aren't any significant counties with both a high percentage of minors and elderly, there are regions in comparison to the rest of the data where there aren't many hospital beds. Standardizing the hospital bed counts uncovers multiple counties with a higher minors/elders population with about the same number of beds per 1000 people as counties with lower numbers of these age groups like Sumter County, Fl whose population is 66% people over 60 with only 2.6 beds/1000 people. Health officials in counties like Sumter, Fl and Charlotte, Fl where there's a higher percentages of people over 60 and relatively low standardized bed counts should prepare more resources and enact stricter policies in preventing and controlling the spread.
![Unknown](https://user-images.githubusercontent.com/60996310/80255491-056e3800-864b-11ea-899d-548382167408.png)

The **heat map** conveys how there is no significant correlation in the number of hospital beds and COVID19-related deaths (correlation of almost 0) while conveying a slightly positive correlation with the number of deaths and the population size (of all ages). There are also low correlations between other factors like dependency ratios. This suggests that these variables don't play a large role in determining what considers a county more at risk and encourages exploring other data sources on potential contributing factors like number of human resources (i.e. healthcare workers), social vulnerability (i.e. accessibility to housing/transportation), or medical supplies. 

<img width="1317" alt="Screen Shot 2020-04-24 at 4 49 11 PM" src="https://user-images.githubusercontent.com/60996310/80255751-934a2300-864b-11ea-822b-a9cece960d44.png">


## Business Answer
Although the scatter chart displays the clear disadvantage of some counties with more fragile age groups and low hospital bed counts (i.e. Sumter County, Fl, Charlotte County, Fl), the heat map reveals that these variables aren't very consequential in determining the county's vulnerability level and preparedness in response to COVID-10. It's more helpful to focus on the bar chart data displaying counties with the highest total population (Los Angeles County, CA; Cook County, IL) , highest percentage of people under 18 (Fresno County, CA; Kern County, CA), and highest percentage of people over 60 (Lee County, Fl; Sarasota County, Fl) as they have higher correlations and should be most at risk. Princeton researchers suggest that rural counties with a higher population of people over 60 are more at risk as there's limitation in access to medical resources and institutions in addition to an aging population.

In response to the crises, Lee County and Sarasota county officials have rent assistance programs to prevent homelessness as well as relief funds and funds for businesses; they've enforced stricter protocols in sanitation and social distancing. Their people have been assured that their county is prepared to meet demands in public services; other resources are made available like medical hotlines specifically for COVID-19 concerns. Further data analysis may reveal more counties with similar characteristics in which they can implement similar policies to limit the spread while supporting economy health and morale.  

## Further Analysis
Since there's a .86 correlation between the cases per 1000 and deaths per 1000, it might be useful to analyze data on various hospitalization procedures or practices adopted post-infection as other medical resources that may be more vital in helping those sick recover. Looking at datasets revealing the county's resiliency in dealing with disasters may also help as it takes into account factors like homelessness, poverty, access to transportation, etc. which is useful for public officials to take into account when executing new policies. 

### Data Sources
Google Colab: https://colab.research.google.com/drive/1fIVLH0gPid_dHQgQIpLjusz2ntzRTyKi#scrollTo=SIEA2QAKVX5y&uniqifier=1
Johns Hopkins University Center for Systems Science and Engineering: https://github.com/CSSEGISandData/COVID-19
New York Times: https://github.com/nytimes/covid-19-data
American Community Survey: https://data.census.gov/cedsci/table?q=United%20States&g=0100000US,.050000&tid=ACSST5Y2018.S0101&hidePreview=false&vintage=2018&layer=VT_2018_050_00_PY_D1&cid=DP05_0001E&t=Populations%20and%20People
US Census: https://www.census.gov/geographies/reference-files/2018/demo/popest/2018-fips.html
Homeland Infrastructure Foundation-Level: https://hifld-geoplatform.opendata.arcgis.com/datasets/hospitals
We'll be using GoogleColab and the following packages: pandas 1.0.3, numpy 1.81.1, plotly 4.60
**Additional Source** https://www.princeton.edu/news/2020/04/16/princeton-researchers-map-rural-us-counties-most-vulnerable-covid-19
https://cityftmyers.com/1878/Coronavirus
