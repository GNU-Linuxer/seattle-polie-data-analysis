# Seattle City Crime Data Analysis

This data analysis project discovers select trends of crime offenses in Seattle (from 2008 to present), using the crime dataset from Seattle Police Department. I especially want to answer these questions based on several news articles describing certain aspects of crime activities in Seattle, denoted in the background section (within `Final project.ipynb`).
* How the advent of COVID-19 (2020-01-01) resulted in certain offenses becoming more popular,
* Whether crimes against person is more popular than crimes against property,
* What are most frequent offenses in University District, and
* Whether Seattle has record-high homicide offenses counts. 

After data analysis, I discovered that 
* Fraud offense, burglary, vandalism of property, robbery, and weapon law violation have increased after 2020-01-01,
* Crime against property is noticeably more frequent than crime against person,
* Larceny/theft, burglary, and assault offenses are popular in the University District, and
* Seattle do have a record-high homicide offense in 2020 (55 offenses total).

Result from this data analysis encourages readers to take extra care on their properties while in Seattle, and especially be vigilant on fraud attempts. Moreover, these findings helps people in the University District (the University of Washington area) to aware thefts on their laptop computers and other valuable items.

## Dataset Used

City of Seattle Crime Data (2008 - Present) from [Seattle Open Data Website](https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5)

## Dataset Field description

| Field Name | Description | Field is used in my analysis | 
| ---------- | ----------- | ---------------------------- |
| Report_Number | Primary key/UID for the overall report. One report can contain multiple offenses, as denoted by the Offense ID.  | ✘ | 
| Offense_ID | Distinct identifier to denote when there are multiple offenses associated with a single report.  | ✘ | 
| Offense_Start_DateTime | Start date and time the offense(s) occurred.  | ✔️ | 
| Offense_End_DateTime | End date and time the offense(s) occurred, when applicable.  | ✘ | 
| Report_DateTime | Date and time the offense(s) was reported. (Can differ from date of occurrence)  | ✘ | 
| Group_A_B | Corresponding offense group.  | ✘ | 
| Crime_Against_Category | Corresponding offense crime against category.  | ✔️ | 
| Offense_Parent_Group | Corresponding offense parent group.  | ✔️ |  
| Offense | Corresponding offense.  | ✔️ | 
| Offense_Code | Corresponding offense code.  | ✔️ | 
| Precinct | Designated police precinct boundary where offense(s) occurred.  | ✘ | 
| Sector | Designated police sector boundary where offense(s) occurred.  | ✘ | 
| Beat | Designated police beat boundary where offense(s) occurred. | ✘ | 
| MCPP_Neighborhood | Designated [Micro-Community Policing Plans](https://www.seattle.gov/police/community-policing/mcpp) (MCPP) boundary where offense(s) occurred. | ✔️ | 
| Blurred_Address | Offense(s) address location blurred to the one hundred block.  | ✘ | 
| Blurred_Longitude Coordinate | Offense(s) spatial coordinate blurred to the one hundred block.  | ✘ | 
| Blurred_Latitude Coordinate | Offense(s) spatial coordinate blurred to the one hundred block. | ✘ | 


SPD employs an FBI UCR NIBRS-compliant police records management system in accordance with reporting guidelines. For additional information visit https://www.fbi.gov/services/cjis/ucr/nibrs.

[Seattle Open Data Website](https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5) contains an up-to-date PDF file describing all fields in this dataset.

## Generated .csv files

`Question 1-4 out.csv` files are cleaned and processed data prior to statistical analysis and data visualization (for the specific question). Readers can import .csv files to their favorite analysis/visualization software.

## API documentation
* [SODA API documentation](https://dev.socrata.com/consumers/getting-started.html)

Known issue: Readers/Users may need to sign-up for App token on [this data.seattle.gov link](https://data.seattle.gov/profile/edit/developer_settings); otherwise their requests are subject to rate limitation. Optional code and instruction to import App token is denoted in the `Final project.ipynb` notebook file.

## License

* Code, Python Notebook, and generated .csv files are licensed under MIT license.
* Dataset is licensed under Public Domain.

## Other Related Data Analysis Reports

* [Exploring Seattle Crime](https://cse412-21w.github.io/seattle-crime/), a UW CSE 412 Data Visualization Project