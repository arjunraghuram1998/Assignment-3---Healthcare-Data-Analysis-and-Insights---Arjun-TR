# Assignment-3---Healthcare-Data-Analysis-and-Insights---Arjun-TR
 Healthcare Data Analysis and Insights - Arjun TR
ASSIGNMENT 3


The Given Data Sheet has been loaded to Power Query

Data Cleaning:

1. Checking the number of missing values marked with '?' in each column of the “Medical 
Examinations” Table and "Hospitalization Details" Table. 

Medical Examinations table having - 2 
Hospitalization Details table having - 13

"?" replaced with null

2.Missing values of ‘month’ replaced with Sep, Missing values in year replaced with average 1983

3. Most frequently occurring values in the ‘smoker’, 'Hospital tier' and 'City 
tier' columns, are replaced with mode.

4.'State ID' values are missing, filled with "Unknown"


Data Transformation:

1.‘names’ column in the “Customer Names” Table into 3 meaningful columns: ‘Title’, ‘First Name’, and ‘Last Name’. has been splited.

2."NumberOfMajorSurgeries" column in the “Medical Examinations” Table to numerical data by replacing non-numeric characters with meaningful numerical values. (0)

3.Inconsistencies in the 'Heart Issues' and 'smoker' columns, using Trim, Clean, Capitalize.

4.New column named “Weight Status” created and funtions added to show weight categories

5. new column named “Diabetes Status” - created and funtions added to show Diabetes range.

6. Merge ‘year’, ‘month’ and ‘date’ columns in the “Hospitalization Details” Table into one 
column named ‘Date of Birth’ - created and format it in ‘DD-MMM-YYYY’ custom format, Done  

7.the ‘Age’ of each customer based on their ‘Date of Birth’ and the date of 
collection of the dataset, which is 8thJune 2023.=DATEDIF([@[Date of Birth]],"8/june/2023","Y")

8.Format ‘charges’ column as currency ($). 


Data Exploration, Analysis & Visualization

A new sheet named “Healthcare" created and Using VLOOKUP Function 3 sheets combined to 1 sheet

Analysis using Pie/Donut Chart:  

Analysis using Pie/Donut Chart, the distribution of cancer history among smokers and non-smokers
Analysis of number of major surgeries and average HbA1C differ between patients with and without a history of transplants

Analysis using Column/Bar Chart:  

Healthcare charges vary based on different weight statuses and diabetes statuses are visualised through column chart
The average charges for each hospital tier within different states are visualised through column chart

Analysis using Line/Scatter Plot

1.Correlation between age and both BMI and HbA1C in the dataset - Visualised by Line Chart
2.Relationship between age and healthcare charges - Visualised by Line Chart

Dashboard Creation 

Add slicers for the fields “Weight Status” and “Diabetes Status” to enable filtering across 
all visualizations, supporting comparison of health outcomes and charges based on body 
weight and diabetes condition - Done
