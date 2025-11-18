# Consumer Complaint Data Analysis – Summary

**Objective:**
To analyze nationwide consumer complaint records, clean the dataset, standardize fields, and derive meaningful insights related to complaint trends, company performance, and customer grievance status.

**Key Tasks Performed**
* Cleaned and standardized inconsistent fields such as State, Issue, Product, Date Received, Date Resolved.
* Removed duplicates, handled missing values, and validated date formats.
* Extracted useful time-based fields such as Year, Quarter, Response Time, etc.
* Performed data segmentation using PivotTables.
* Built summary reports to identify top companies with complaints, product-wise issues, and state-wise distribution.

**Important Formulas Used**
  
* Extracting Year	                                   =YEAR([@Date Received])
* Extracting Quarter	                                 ="Q"&ROUNDUP(MONTH([@Date Received])/3,0)
* Calculating Resolution Days	                       =[@Date Resolved] - [@Date Received]
* Text Standardization	                               =TRIM(), =PROPER(), =UPPER()
* Creating Categorization	                           =IF(condition, value_if_true, value_if_false)
* Counting Complaints (conditions)	                   =COUNTIFS(Range1,Criteria1,Range2,Criteria2)
* Summing Amounts (conditions)	                       =SUMIFS(SumRange, Range1, Criteria1)
* Lookup Company/State Information	                   =VLOOKUP(), =XLOOKUP()
* Detecting Missing Values	                           =IF(ISBLANK(cell),"Missing","OK")
* Merging Text Fields	=CONCAT(),                     =TEXTJOIN()

**Excel Tools/Techniques Used**

* PivotTables & PivotCharts
* Data Cleaning (Remove Duplicates, Flash Fill, Text-to-Columns)
* Conditional Formatting for insights
* Data Validation for standardized categories
* Slicers for dashboard interactivity
* Advanced filters
* Sorting & grouping by dates

**Takeaways**

* we can see in horizontal bar chart that which issue is priority
* in trend line we can see that april,july and august has most no. of complaints
* in timely response bar chart we can see its declining , which is not good
* average resolution time is decresing , that’s good
* total no. of complaint is decreasing every year

