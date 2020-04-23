# Management for COVID19 Pandemic Through Python Data Analysis
COVID19 is a newly discovered infectious disease that's spreading illness, fear, and uncertainty in all sectors of society. 
It's a challenge for individuals, businesses, organizations, and governments which makes it particularly crucial for data analysis on existing and updating information on the virus characteristis, age/sex groups that are more at risk,resources available, and effects on important institutions. 
Effective data management can help minimize these the effects and help decision-makers better allocate resources and attention given the trends. 

**Business Question**
Based on demographics and hospital availability, which FIPS counties are the most vulnerable or at risk during COVID19?

It's important to address this to allow policymakers in each region to implement practices like social distancing and businesses to prepare workers and supplies to support these weaker areas. 

**Data Question**
What metrics and data do we have to monitor healthcare resources and COVID19 conditions in the given counties?

## Analysis
![](Bar_Tot_Pop)
The bar chart conveys 20 counties with the highest populations with Los Angeles County, California taking a significant lead at 10.1M; its high number of people suggests that the county is most at risk for virus transmission, but zoning into population density and certain characteristics reveal that although certain counties are less populated, they may be more at risk. For example, the following chart manifests the top 20 counties with the highest percentages of people over 60, a vulnerable age group. 

In the bubble chart, it's seen that although there aren't any significant counties with both a high percentage of minors and elderly, there are regions in comparison to the rest of the data where there are not many hospital bed counts. Standardizing the hospital bed counts uncovers multiple counties with a higher minors/elders population with 


**Business Answer**

### Data Sources
Google Colab: https://colab.research.google.com/drive/1fIVLH0gPid_dHQgQIpLjusz2ntzRTyKi#scrollTo=SIEA2QAKVX5y&uniqifier=1
Johns Hopkins University Center for Systems Science and Engineering: https://github.com/CSSEGISandData/COVID-19
New York Times: https://github.com/nytimes/covid-19-data
American Community Survey: https://data.census.gov/cedsci/table?q=United%20States&g=0100000US,.050000&tid=ACSST5Y2018.S0101&hidePreview=false&vintage=2018&layer=VT_2018_050_00_PY_D1&cid=DP05_0001E&t=Populations%20and%20People
US Census: https://www.census.gov/geographies/reference-files/2018/demo/popest/2018-fips.html
Homeland Infrastructure Foundation-Level: https://hifld-geoplatform.opendata.arcgis.com/datasets/hospitals
We'll be using GoogleColab and the following packages: pandas 1.0.3, numpy 1.81.1, plotly 4.60
