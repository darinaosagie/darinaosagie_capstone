# darina_capstone

**Capstone for Nashville Software School Data Analytics Program**
**Completion date: August 18, 2022**

**Overview**
According to the Center for Disease Control (CDC), prescription opioids were involved in nearly 24% of all opioid overdose deaths in 2020, which was a 16% increase in prescription opioid-involved deaths from 2019 to 2020.

The CDC categorizes prescription opioid overdose deaths into three sections:
1.	Natural opioids: Pain medications like morphine and codeine.
2.	Semi-synthetic opioids: Pain medications like oxycodone, hydrocodone, hydromorphone, and oxymorphone.
3.	Methadone: A synthetic opioid used to treat pain, but it can also be provided through opioid treatment programs to treat opioid use disorders.
Regarding the state of Tennessee for 2019 and 2020 - this project aims to identify if counties with lower income per capita have a higher rate of fatal overdoses due to semi-synthetic opioids compared to higher-income counties and if counties with lower income per capita have higher number of opioid pills prescribed compared to wealthier counties.

**Data Question**
1.	What is a MAT Center? Where are TN MAT centers located? 
2.	What is the income per capita for each county? What was the annual percentage variation?
3.	What is the total amount of fatal prescription opioid overdoses per county? What was the annual percentage variation?
4.	What is the total amount of pills prescribed for Hydrocodone, Oxycodone and Tramadol per county?  What was the annual percentage variation?
5.	What is the total number of overdoses for Hydrocodone, Oxycodone and Tramadol per county? What was the annual percentage variation?

**Methodologies**
**1. Gathering the Data**
Using data from the Tennessee Department of Health website, I obtained information in Excel format about MAT center locations, prescription numbers, overdose numbers, and a data dictionary categorizing types of overdoses.
I also acquired median income per capita data for each county and its respective year from the US Census Bureau.

**2. Analyzing and Cleaning the Data**
Data cleaning became necessary when I discovered that the Tennessee Department of Health had overdose information for all 95 counties within the state from 2017 to 2022. This database included ten different types of overdose categorizations along with overdose counts for each category. To clean this data, I first consulted the data dictionary to identify which types of overdoses applied to opioid information. Then, I filtered the data for my desired years and counties, and subsequently aggregated the counts of each overdose type by category.
Regarding the US Census Bureau information, data cleaning proved to be tedious as county information was stored in separate CSV files, each containing 120 pieces of data for every county, categorized by year. Initially, I began data cleaning using Python, but later transitioned to Excel. First, I downloaded and converted the 2019 data to Excel format, enabling me to filter for specific needs like income per capita and population. I repeated this process for the year 2020 as well.

**Visualizing the Data**
Tableau was utilized to create clear and concise visualizations in a storytelling format. Two types of charts were utilized: bar charts, which effectively displayed the annual variations in income per capita, total overdose numbers, and the prescribed opioid pill count for each county; and distribution charts, which were used to identify correlations between income per capita and total overdoses, as well as between income per capita and the total number of prescribed pills per county, categorized by pill type.

**Technologies Used**
Python - pandas, numpy, seaborn, matplotlib, cleaning data
Tableau – visualizations
Excel – cleaning data

**Data Sources**
MAT Treatment Center Locations, Prescription Data, Fatal Overdoses Data: Tennessee Department of Health 
Median Income Per Capita Data: United States Census Bureau 
Tennessee Counties Ranked Per Capita Income: Wikipedia 

**Conclusion**
While answers to the initial research questions were inconclusive, the data highlights patterns for the Tennessee State Opioid Treatment Department to consider regarding MAT Centers in Jackson County. 
Jackson county had the lowest income per capita throughout this dataset ($33,336 in 2019, $36,084 in 2020). However, it stood out as an outlier in all overdose categories. 
All Opioid Overdoses: 0.08 to 0.16 per 1,000 (2020). 
All Prescription Opioids: Stable at 0.16 (2019-2020). 
All Opioids & Stimulants: 0.16 (2019-2020). 
All Opioids & Benzodiazepines: 0.00% to 0.16 (2019-2020). 
Next Steps
The Tennessee State Opioid Treatment Department could consider establishing an additional Medication-Assisted Treatment (MAT) center in Jackson County, which currently has only one center serving the area. This move could address the unique overdose patterns observed in the county.
