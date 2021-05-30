# Seattle City Crime Data Analysis

This data analysis project compares the trend of US Stock market and Cryptocurrency market throughout 2016-04-01 till 2021-3-31, for the sake to analyze whether two markets correlates (or inversely correlates) with each other, and how COVID-19 Pandemic changes such correlation. Bitcoin and other cryptocurrencies have become a more and more popular alternative investment vehicle (than the US Stock market), especially during the COVID-19 pandemic that has brought Bitcoin's price from $6000 to $6000**0** at one point. Result from this data analysis can inform readers how similar (or different) does the US Stock market and Cryptocurrency market behave, which might provide them useful information when they're investing in either market.

## Dataset Used

City of Seattle Crime Data (2008 - Present) from [Seattle Open Data Website](https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5)

## Dataset Field description

| Field Name | Description | Field is used in my analysis | 
| ---------- | ----------- | ---------------------------- |
| Report_Number | Primary key/UID for the overall report. One report can contain multiple offenses, as denoted by the Offense ID.  | ✖️ | 
| Offense_ID | Distinct identifier to denote when there are multiple offenses associated with a single report.  | ✖️ | 
| Offense_Start_DateTime | Start date and time the offense(s) occurred.  | ✔️ | 
| Offense_End_DateTime | End date and time the offense(s) occurred, when applicable.  | ✖️ | 
| Report_DateTime | Date and time the offense(s) was reported. (Can differ from date of occurrence)  | ✖️ | 
| Group_A_B | Corresponding offense group.  | ✖️ | 
| Crime_Against_Category | Corresponding offense crime against category.  | ✔️ | 
| Offense_Parent_Group | Corresponding offense parent group.  | ✔️ |  
| Offense | Corresponding offense.  | ✔️ | 
| Offense_Code | Corresponding offense code.  | ✔️ | 
| Precinct | Designated police precinct boundary where offense(s) occurred.  | ✖️ | 
| Sector | Designated police sector boundary where offense(s) occurred.  | ✖️ | 
| Beat | Designated police beat boundary where offense(s) occurred. | ✖️ | 
| MCPP_Neighborhood | Designated [Micro-Community Policing Plans](https://www.seattle.gov/police/community-policing/mcpp) (MCPP) boundary where offense(s) occurred. | ✔️ | 
| Blurred_Address | Offense(s) address location blurred to the one hundred block.  | ✖️ | 
| Blurred_Longitude Coordinate | Offense(s) spatial coordinate blurred to the one hundred block.  | ✖️ | 
| Blurred_Latitude Coordinate | Offense(s) spatial coordinate blurred to the one hundred block. | ✖️ | 


SPD employs an FBI UCR NIBRS-compliant police records management system in accordance with reporting guidelines. For additional information visit [https://www.fbi.gov/services/cjis/ucr/nibrs].

[Seattle Open Data Website](https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5) contains an up-to-date PDF file describing all fields in this dataset.

## Generated .csv files

Question 1-4.csv files are cleaned and processed data prior to statistical analysis and data visualization (for the specific question). Readers can import .csv files to their favorite analysis/visualization software.

## API documentation
* [SODA API documentation](https://dev.socrata.com/consumers/getting-started.html)

Known issue: Readers/Users may need to sign-up for API key on [data.seattle.gov] ; otherwise their requests are subject to rate limitation. Optional code and instruction to import API key is denoted in the `Final project.ipynb` notebook file.

## License

* Code, Python Notebook, and generated .csv files are licensed under MIT license.
* Dataset is licensed under Public Domain.