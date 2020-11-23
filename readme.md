## ASA Data Challenge Expo
### Introduction

* Name: Walter Yu
* Date: Fall 2020

This notebook is the contest entry to the [ASA Data Challenge Expo][00.00] to help citizens and communities response to COVID-19 with U.S. Census data analysis from the sources listed in the following sections.

[00.00]: https://community.amstat.org/dataexpo/home

### Data Sources

Both core and supplemental datasets from the [problem statement][00.01] were used for this analysis. Data was downloaded from portal websites as follows:

1. U.S. Census Website: Advanced [search feature][00.02] was used to filter data in the following order: Surveys > Years > Geography > Topics
2. U.S. Census COVID-19 Website: CA state data was downloaded from the [categorical dataset search page][00.03]

[00.01]: https://opportunity.census.gov/assets/files/covid-19-top-asa-problem-statement.pdf
[00.02]: https://data.census.gov/cedsci/advanced
[00.03]: https://covid19.census.gov/

### Core Datasets

1. 2019 American Community Survey (ACS) Single-Year Estimates - Language Spoken
* Description: PLACE OF BIRTH BY LANGUAGE SPOKEN AT HOME AND ABILITY TO SPEAK ENGLISH IN THE UNITED STATES
* Survey/Program: American Community Survey
* Years: 2019,2018,2017,2016,2015,2014,2013,2012,2011,2010
* Table: [B06007][01.00]

[01.00]: https://data.census.gov/cedsci/table?q=B06007&tid=ACSDT1Y2019.B06007

2. 2019 American Community Survey (ACS) Single-Year Estimates - Household Income
* Description: HOUSEHOLD INCOME IN THE PAST 12 MONTHS (IN 2019 INFLATION-ADJUSTED DOLLARS)
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B19001][01.01]

[01.01]: https://data.census.gov/cedsci/table?text=B19001&tid=ACSDT1Y2019.B19001

3. 2019 American Community Survey (ACS) Single-Year Estimates - Median Household Income
* Description: MEDIAN HOUSEHOLD INCOME IN THE PAST 12 MONTHS (IN 2019 INFLATION-ADJUSTED DOLLARS)
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B19013][01.02]

[01.02]: https://data.census.gov/cedsci/table?text=B19013&tid=ACSDT1Y2019.B19013

4. 2019 American Community Survey (ACS) Single-Year Estimates - Poverty Status
* Description: POVERTY STATUS IN THE PAST 12 MONTHS BY SEX BY AGE
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B17001][01.03]

[01.03]: https://data.census.gov/cedsci/table?text=B17001&tid=ACSDT1Y2019.B17001

5. 2019 American Community Survey (ACS) Single-Year Estimates - Housing Cost
* Description: MONTHLY HOUSING COSTS
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B25104][01.04]

[01.04]: https://data.census.gov/cedsci/table?text=B25104&tid=ACSDT1Y2019.B25104

6. 2019 American Community Survey (ACS) Single-Year Estimates - Education Attainment
* Description: EDUCATIONAL ATTAINMENT FOR THE POPULATION 25 YEARS AND OVER
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B15003][01.05]

[01.05]: https://data.census.gov/cedsci/table?text=B15003&tid=ACSDT1Y2019.B15003

7. 2019 American Community Survey (ACS) Single-Year Estimates - Commute Mode
* Description: MEANS OF TRANSPORTATION TO WORK BY AGE
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B08101][01.06]

[01.06]: https://data.census.gov/cedsci/table?text=B08101&tid=ACSDT1Y2019.B08101

8. 2019 American Community Survey (ACS) Single-Year Estimates - Race
* Description: RACE
* Survey/Program: American Community Survey
* Years: 2019
* Table: [B02001][01.07]

[01.07]: https://data.census.gov/cedsci/table?text=B02001&tid=ACSDT1Y2019.B02001

### Supplemental Datasets

1. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [California Counties DP02 Social][02.00]

[02.00]: https://covid19.census.gov/datasets/california-counties-dp02-social

2. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [California Counties DP03 Economic][02.01]

[02.01]: https://covid19.census.gov/datasets/california-counties-dp03-economic

3. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [California Counties DP04 Housing][02.02]

[02.02]: https://covid19.census.gov/datasets/california-counties-dp04-housing

4. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [California Counties DP05 Demographic][02.03]

[02.03]: https://covid19.census.gov/datasets/california-counties-dp05-demographic

5. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [Household Pulse Survey Public Use File][02.04]

[02.04]: https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html

6. U.S. Census - COVID-19 Demographic and Economic Resources
* Dataset: [COVID-19 Case Surveillance Public Use Data][02.05]

[02.05]: https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data/vbim-akqf

### Geospatial Datasets

1. U.S. Census - COVID-19 Demographic and Economic Resources
* Description: American Community Survey (ACS) about household income ranges and cutoffs and Poverty Status.
* These are 5-year estimates shown by state and county boundaries.
* Link: [Dataset][03.00]

[03.00]: https://uscensus.maps.arcgis.com/home/item.html?id=b2ba19b4cce04a9796d9cdeecaba2f18

2. U.S. Census - COVID-19 Demographic and Economic Resources
* Description: American Community Survey (ACS) about household income ranges and cutoffs.
* These are 5-year estimates shown by county, and state boundaries.
* Link: [Dataset][03.01]

[03.01]: https://uscensus.maps.arcgis.com/home/item.html?id=0fbb1571e5b6458f941580d1d64a6693

3. U.S. Census - COVID-19 Demographic and Economic Resources
* Description: American Community Survey (ACS) about total population count by sex and age group.
* These are 5-year estimates shown by state and county boundaries.
* Link: [Dataset][03.02]

[03.02]: https://uscensus.maps.arcgis.com/home/item.html?id=eab0f44ba5184c609175caa7ae317f0c
