## Helping Communities During the COVID-19 Pandemic

### Entry Details

* [ASA Data Challenge Expo][00.00]
* Name: Walter Yu
* Date: Fall 2020

[00.00]: https://community.amstat.org/dataexpo/home

### Executive Summary

This entry aims to help disadvantaged communities during the COVID-19 pandemic by answering the following questions:

1. Explore the relationship between socioeconomic features of the U.S. population and disadvantaged communities.
2. Identify disadvantaged communities based on their median household income and socioeconomic factors.
3. Identify which disadvantaged communities have been most impacted by the COVID-19 pandemic and in need of public services.
4. Provide recommendations on helping these communities based on data analysis results.

The intended audience are state/local governments, non-governmental organizations (NGOs) and volunteers which are able to provide aid and services to these communities.

### Scope

This entry focuses on California communities to control its scope since several questions are being considered, and data analysis of all U.S. communities would expand the scope and length of this report. This limited scope provides for more detail and attention to be paid to analysis, documentation and recommendations.

## Part 1: Overview

### Methodology

This entry is designed to be interpretable, so it clearly outlines data analysis steps into the following modules:

1. Overview: Outline approach, assumptions and data sources
2. Data Processing: Data preparation and manipulation for analysis
3. Data Analysis: Model fit, coefficient interpretation and diagnostics
4. Data Visualization: Communicate findings through data plots  
5. Recommendations: Document key findings from data analysis

### Assumptions

This entry makes the following assumptions:

1. Although the scope is limited to California communities, the methodology can be applied to other states since it is based on data extracted from the U.S. Census for the state/county level and do not contain any characteristics specific to California.
2. State and federal [guidelines][00.11] typically define disadvantaged communities as being low-income, so median household income was used to identify such communities.
3. Data analysis was documented to be clear and easily interpretable, so linear regression and the [Law of Parsimony][00.12] were applied whenever possible

[00.11]: https://www.hud.gov/topics/rental_assistance/phprog
[00.12]: https://en.wikipedia.org/wiki/Occam%27s_razor

### Data Summary

This entry analyzes core and supplemental datasets from the data challenge [problem statement][00.01] as follows:

* Core Dataset: 2019 American Community Survey (ACS) Single-Year Estimates
* Supplemental Dataset: COVID-19 Data from the National Center for Health Statistics

Data was downloaded from portal websites as follows:

1. U.S. Census Website: Advanced [search feature][00.02] was used to filter data in the following order: Surveys > Years > Geography > Topics.
2. U.S. Census COVID-19 Website: CA state data was downloaded from the [categorical dataset search page][00.03].
3. National Center for Health Statistics (NCHS) Website: Death counts by county and race downloaded from their [data portal][00.04].

[00.01]: https://opportunity.census.gov/assets/files/covid-19-top-asa-problem-statement.pdf
[00.02]: https://data.census.gov/cedsci/advanced
[00.03]: https://covid19.census.gov/
[00.04]: https://www.cdc.gov/nchs/covid19/index.htm

### Core Datasets

Datasets of interest were identified from the U.S. Census data portal and extracted using the advanced search tool. Table ID numbers are listed for reference.

1. 2019 American Community Survey (ACS) Single-Year Estimates - Language Spoken
* Description: PLACE OF BIRTH BY LANGUAGE SPOKEN AT HOME AND ABILITY TO SPEAK ENGLISH IN THE UNITED STATES
* Survey/Program: American Community Survey
* Years: 2019
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

### Supplemental Datasets (U.S. Census)

Datasets of interest were identified from the U.S. Census COVID-19 data portal under the categorical dataset section.

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

### Supplemental Datasets (NCHS)

Datasets of interest were identified from the National Center for Health Statistics (NCHS) data portal.

1. NCHS - COVID-19 Data from the National Center for Health Statistics
* Dataset: [Provisional COVID-19 Death Counts by County and Race][02.06]

[02.06]: https://data.cdc.gov/NCHS/Provisional-COVID-19-Death-Counts-by-County-and-Ra/k8wy-p9cg

### Geospatial Datasets

Datasets of interest were identified from the U.S. Census COVID-19 data portal under the categorical dataset section.

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
