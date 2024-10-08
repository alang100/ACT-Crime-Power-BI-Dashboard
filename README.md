## ACT Crime Power BI Dashboard
I have used  the ACT crime dataset from a university project to create a Power BI dashboard for ACT crime. Two dashboards were made for the two datasets.

The source of the datasets are the ACT polive website
https://www.policenews.act.gov.au/crime-statistics-and-data/crime-statistics


This project consisted of the following:

**Data wrangling:** The original csv files are provided in this repository as are the wrangled files. Wrangling for the 2022 dataset was done in excel.
Additional population data was obtained from the ABS website for the 2021 census.
Coordinate data for suburbs and districtis were found on an ACT government website. Many coordinates have been modifed by observing them in google maps and choosing an appropriate set of coordinates.  

A Python Jupyter notebook script has been developed to automatically wrangle the XLS file from the crime-statistics website. The input files are 'Website Stats Monthly Download.xlsx' and 'District Population.xlsx' which contains the district population from the 2021 census.  

The output file created is 'Website Stats Monthly Wrangled.xlsx' which is the file that is directly loaded by the 2024 ACT Crime Stats dashboard.

**Power query:** Many steps were taken within power query, they can be observed in the pbix files.

**Power BI:** Many measures were created to calculate certain numbers such as 'crimes per month' and crimes per annum per 1000 residents'. 

### ACT Crime Stats June 2022 Dataset

This format of the dataset was available up until June 2022.
Incident numbers are given for an entire quarter. 
In the Date slicers, the date is the last day of the quarter. 
There are statistics for 23 infringement types.
Statistics are given by suburb, offering detailed granularity for the maps.
The two Location tabs are the same except for the map format. Ideally, I would have liked to combine the two formats(map 1 maps and map 2 polygons, but that is not possible in the free version of Power BI.
The available dataset after June 2022 could no longer be broken down by suburb.


### ACT Crime Stats June 2024 Dataset
This format of the dataset has been available since July 2022.
Incident numbers are given for every month starting from January 2014. 
In the Date slicers, the date is the last day of the month. 
There are statistics for 23 infringement types.
Statistics are no longer given by suburb, but rather by district. 
Statistics of only 13 infringement types are broken down by district.




