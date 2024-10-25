## PROJECT TITLE: COFFEE SHOP SALES DATA ANALYSIS

1. Table Of Contents
2. Project Overview
3. Data Analysis
4. Tools And Technique
5. Formulars Used
6. Insights
7. Recommendation
8. Dashboard Design



## PROJECT OVERVIEW
As a data analyst, analyze the coffee shop data to identify trends, Customer insights and geographical sales patterns and create a dynamic dashboard with filtering options.

### Data Analysis 
•	Data Cleaning: Checking for missing Data/Errors
•	Imported the needed columns using XLOOKUP from Other tables (Customers and product) into Orders Table. The orders Table contains the Order date, and the IDs which makes it easy to call up columns from the other tables.
•	The imported Columns are Unit Price, Profit, Size, Roast Type, Coffee Type, Loyalty Card, Country
•	Use the Unit price and Quantity to calculate the Total sales by multiplying them both. 
•	From the Date in the Order table, I Separated the Year, Month, Day, on individual columns
•	Pivot table was inserted on a new sheet to create a trend for Total Sales, Coffee Type was placed on column and Year was added to the Row. This table was used to create a Line Chart to show the trend.
•	A Pivot table was used to analyze the Customers Names based on their Contribution to the Total Sales. This was later used to create a Clustered Column Pivot Chart.
•	A Pivot table was used to analyze the Total sales by each country and finally converted into a Pie Chart.
•	A Pivot table was used to analyze the quantity ordered for each Coffee Type; a 3D Clustered Bar was used to represent the analysis.  

Slicers
I created Four (4) different slicers on a different sheet.
•	The year slicer
•	The Loyalty Card slicer
•	The Roast Type slicer
•	The size slicer

Dashboard
•	On a New Sheet, go to new View to switch off the Gridline. 
•	Inserted a downloaded coffee image, increase the transparency of the image. This is to serve as a Background. 
•	Then create a background for the dashboard itself, using a rounded rectangular box, format the box so it has No fill also reduce the roundness of the edges.
shape fill - black
 Shape outline - No outline
Increase the transparency to 10%
•	Then start bringing in the Pivot Charts
•	Arrange the charts as you wish, giving space for the Metrics and title/Heading above the charts.
•	Organizing the charts properly fit the dashboard  
•	Bring in the Coffee Cup which is to be used as the LOGO. 
•	Then Insert Text box, to input Title, use Shape No fill to remove the background default color.
•	Bring in the previously created slicers, Format the slicers and change color to ash to suit our color.
•	Connect the slicers with all the charts on the dashboard.
•	Arrange the slicers on the Left side of the dashboard.

Heading
•	Bring in a text box for the title, write the Title you want, and format the text box. 
•	Bring in a text box to add the metric, also bring in text boxes for the metrics names and arrange to fit the heading space. 

### Tools And Technique
Microsoft Excel (data analysis and visualization)
Data manipulation and filtering techniques
Pivot Chart and Pie Charts 
Presentation software (PowerPoint)

### FORMULARS USED
1. Year =TEXT([@[Order Date]],"YYYY")
2. Month =TEXT([@[Order Date]],"MMM")
3. Total Sales =[@Quantity]*[@[Unit Price]]
4. Profit from Product Table =XLOOKUP([@[Product ID]],products!$A$2:$A$49,products!$G$2:$G$49)
5. Size =XLOOKUP([@[Product ID]],products!$A$2:$A$49,products!$D$2:$D$49)
6. Roast Type =XLOOKUP([@[Product ID]],products!$A$2:$A$49,products!$C$2:$C$49)
7. Coffee Type =XLOOKUP([@[Product ID]],products!$A$2:$A$49,products!$B$2:$B$49)
.  Loyalty Card =XLOOKUP([@[Customer ID]],customers!$A$2:$A$1001,customers!$I$2:$I$1001)
9. Country =XLOOKUP([@[Customer ID]],customers!$A$2:$A$1001,customers!$G$2:$G$1001)
10. Customers Name =XLOOKUP([@[Customer ID]],customers!$A$2:$A$1001,customers!$B$2:$B$1001) 
11. Sum of all Total Profit =SUM([Profit])
12. Sum of All Total Sales =SUM([Total Sales])
13. Sum of all Quantity sold =SUM([Quantity])

## INSIGHTS 
Key Insights from the analysis is 
1.	A notable decline in sales revenue was observed in 2022, deviating from the overall trend across the four-year analysis period. 
2.	Our Analysis confirms that the united state as the largest consumer market with a 79% sales share. 
3.	The Ara Coffee type is the most consumed coffee type. 
4.	Surprisingly, non-loyalty card holders accounted for 71%, i.e. 5 of our top 7 customers, revealing that loyalty cards are not a definitive indicator of high value customers. 

## RECOMMENDATION
1.	Consider alternative loyalty programs focusing on rewards and personalized offers.
2.	To analyze demographics, purchase frequency and pattern to identify high value customer segment.
3.	Develop marketing strategies to engage and retain top spending customers without loyalty cards. 
4.	Investigate and analyze drivers of non-loyalty cardholders purchasing behavior.
5.	Continuously analyze sales data to identify areas for improvement.





 

