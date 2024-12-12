<img src="https://cdn.theatlantic.com/thumbor/AZnX7vSCab-KUUUnomXVV_AtE5I=/1200x807/media/img/photo/2020/05/kentucky-photos/a01_1164037780/original.jpg" width="1000" height="500">

# Preventative Healthcare in Kentucky
An examination of the types and percentages of preventative healthcare accessible to Kentucky residents by county using CDC data from 2022 and USDA poverty rate data from 2021.

### Summary
This project analyzes the 2021 estimated poverty rates across Kentucky’s 120 counties in relation to the estimated rates of preventive healthcare received by county residents in 2022. The preventive healthcare data encompasses routine services such as annual physical exams, age-appropriate cancer screenings, and dental visits within the past 12 months. Additionally, the analysis includes estimates of the adult populations in each county without any access to healthcare. The aim of this study is to examine the correlation between poverty rates and a lack of preventive healthcare, as well as to identify which county populations have the greatest need for improved access to various forms of preventive care.

### Conclusions 
While there is a clear correlation between poverty rates in Kentucky's counties and a lack of preventive care, poverty and lack of insurance do not appear to be the sole factors. For instance, Oldham County had an estimated poverty rate of 4.9% in 2021, and only 4.7% of the population lacked health insurance in 2022. However,  only an estimated 68.6% of the county's residents visited a dentist in the past 12 months, with the percentage only decreasing across other counties in Kentucky. This lack of dental care may be due to financial constraints, insurance coverage issues, or simply a lack of awareness about the importance of regular dental exams.  

Furthermore, poverty rates are notably higher in the southeastern region of Kentucky, especially in counties bordering Virginia and West Virginia. This increase can be linked to the decline of the coal industry in the area, coupled with a lack of viable replacement industries. However, high poverty rates do not necessarily correlate with a lack of preventive healthcare. For example, Martin County had the highest poverty rate in Kentucky in 2021 at 40.5%, but 74.8% of its population completed their annual checkup in 2022. Meanwhile, only 41.2% of the county population had visited a dentist within the past year in 2022. These examples suggest that financial factors alone cannot explain the lack of preventive care utilization. Other factors, such as transportation, the availability of in-network providers, and access to health resources, must also be considered when examining preventative healthcare rates.

### Feature List


## Kentucky Healthcare & Poverty Data Dictionary
### Overview
Project Name: Kentucky Preventative Healthcare & Poverty Analysis by County 2021-2022  
Version: 1.0  
Last Updated: 12/08/2024  
Purpose: Track and analyze poverty rates and healthcare metrics across Kentucky counties to determine what type of care is needed and in what region. 

### Dataset Information
#### Primary Dataset  
Records: 120 counties   
Format: CSV/Excel  
Update Frequency: Annual  

### Field Definitions
#### Core Fields
| Field Name | Data Type | Description | Valid Range | Required | Example |
|------------|-----------|-------------|-------------|----------|---------|
| County | Text | Kentucky county name | Valid KY county names | Yes | Adair |
| State | Text | US state name | Kentucky | Yes | Kentucky |
| Year | Integer | Year of data collection | 2021-2022 | Yes | 2021-2022 |
| Poverty Rate Estimate | Decimal | Percentage of population below poverty line | 0.0-100.0 | Yes | 16.0 |
| Annual Checkup | Decimal | Visits to doctor for routine checkup within the past year among adults | 0.0-100.0 | Yes | 76.9 |
| Colorectal Cancer Screening | Decimal | Colorectal cancer screening among adults aged 45–75 years | 0.0-100.0 | Yes | 56.1 |
| Dental Visit | Decimal | Visited dentist or dental clinic in the past year among adults | 0.0-100.0 | Yes | 55.2 |
| Lack of Health Insurance | Decimal | Current lack of health insurance among adults aged 18-64 years | 0.0-100.0 | Yes | 6.1 |
| Mammography | Decimal | Mammography use among women aged 50-74 years | 0.0-100.0 | Yes | 68.8 |


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
  * Be aware of insurance network access restrictions  

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
