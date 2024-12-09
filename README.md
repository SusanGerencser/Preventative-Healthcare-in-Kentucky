# Preventative-Healthcare-in-Kentucky
An examination of the types and percentages of preventative healthcare accessible to Kentucky residents by county using CDC data from 2022 and USDA poverty rate data from 2021.

## Kentucky Healthcare & Poverty Data Dictionary
### Overview
Project Name: Kentucky Preventative Healthcare & Poverty Analysis by County 2021-2022  
Version: 1.0  
Last Updated: 12/08/2024  
Purpose: Track and analyze poverty rates and healthcare metrics across Kentucky counties  

### Dataset Information
#### Primary Dataset  
Records: 120 counties   
Format: CSV/Excel  
Update Frequency: Annual  

### Field Definitions
#### Core Fields
Field Name	Data Type	Description	Valid Range	Required	Example
County	Text	Kentucky county name	Valid KY county names	Yes	"Adair"
Year	Integer	Year of data collection	2021	Yes	2021
Poverty_Rate	Decimal	Percentage of population below poverty line	0.0-100.0	Yes	16.0
Latitude	Decimal	County center latitude	36.4-39.1	Yes	37.8765
Longitude	Decimal	County center longitude	-89.6 to -81.9	Yes	-84.2345

### Geographic Properties
* State: Kentucky
* Number of Counties: 120
* Geographic Level: County

### Data Quality Rules  
  1. Data Validation  
     * No missing county names  
     * Poverty rates must be numeric  
     * All percentages between 0-100  
     * Coordinates must fall within Kentucky boundaries  

  2. Business Rules  
     * One record per county  
     * Current year data only  
     * Standardized county name spelling  

### Technical Specifications
Primary Key: County  
Geographic Identifiers: Latitude/Longitude pairs  
Required Fields: All fields are required  

### Source Information
Data Owner: US Department of Agriculture: Economic Research Service  
Data Owner: CDC: Centers for Disease Control and Prevention      
Data Steward: [usa.gov](https://www.usa.gov/)  
Source Systems:  
* Poverty Data: [Percentage of total population in poverty, 2021: Kentucky](https://data.ers.usda.gov/reports.aspx?ID=17826/)
* Healthcare Metrics: [County Data for 2024 Release](https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb/data/)
* Geographic Data: [Kentucky Counties](https://www.sos.ky.gov/land/resources/Pages/Geographic-Materials.aspx)

### Usage Guidelines
  1. Visualization Requirements  
    * Tableau mapping requires:
      * Clean coordinate data
      * Properly formatted percentages
      * No null values
        
  2. Analysis Considerations  
    * Account for county population differences  
    * Consider rural vs urban factors  
    * Note any seasonal variations  

### Related Documentation
* Kentucky County Boundary Files
* Healthcare Facility Database
* Census Demographic Data
* State Economic Indicators

### Change Log
* Version 1.0

### Initial dataset creation
Base county metrics established  
Geographic coordinates verified  

### Access & Security  
Data Classification: Public  
Access Level: Public  
Security Requirements: None  

### Contact Information
Project Manager: Susan Gerencser  
