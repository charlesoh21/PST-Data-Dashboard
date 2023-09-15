# PST Data Analytics Dashboard


## Overview
PST (Pre-screening Test) data analytics dashboard automatically extracts data from Excel sheets with PST results, transfers data into MySQL database, and generates data analysis and visualizations on Sharepoint.

![image](https://user-images.githubusercontent.com/106832913/184420024-02374655-58f9-4d5b-a810-61e38062c67d.png)


## Dashboard Functionalities
![image](https://user-images.githubusercontent.com/106832913/184422868-c452622d-905e-4392-9add-17e34ade8fdc.png)

1. DIMM Type/Part Number: Selection of DIMM type and part number(s)
2. Product History: Pre-screening test log by date for selected products
3. Selected Parts Information: Total count, avg. failure rate, avg. TTF for selected products
4. Failure Rate Comparison: PST failure rate comparison for selected products
5. DIMM Quantity Proportion by Customers: Customer breakdown for selected products

## Tech Stack 
- Backend: Python 
- Database: SQLite 
- Frontend: Javascript, CSS, HTML
- Libraries: Chart.js, jQuery, lxml

## Moving Data from Excel to Sharepoint
<img src="workflow.PNG"/>

The general flow of data is as seen above. A Python script converts the entries from Excel worksheets to a .db file. This .db file is then converted to a SharePoint list using a mixture of the SOAP and REST APIs provided by SharePoint.


## Impact
1. With analyzed PST data, DSA can provide product quality feedback to DSK 
**-> Increased product quality**
2. Ownership of analyzed PST data will decrease customer management turnaround time by three weeks 
**-> Increased customer satisfaction** 

   **--> Combination of 1 and 2 will lead to a faster qualification of new DIMM products.**
