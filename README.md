# Airlines-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection

## Problem Statement

This dashboard contains the report that was prepared  initially in Tableau and had to be migrated into Power BI. I studied the report as to what visuals are used , DAX used and prepared the same report in Power BI.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a .xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visual filters (Slicers) were added as needed on every Page.
- Step 7 : 5 Pages made are :- Executive view, Customer analysis, Shipping Analysis, Order Sumamary And Sales forecast.
- Step 8 : To calculate Profit ratio, Shipping time and various other needed columns DAX is used in power bi desktop. 
- Step 9 : I tried to stick to what the motive of the Project was and therefore used the same visuals to show the data .
  

  

for creating new column following DAX expression was written;
       
        order days = ABS(Merge1[Ship Date]- Merge1[Order Date])
        Shipment Time = IF(Merge1[order days]>3,"Shipped Late") & IF(Merge1[order days]<3,"Shipped Early") & IF(Merge1[order days]=3,"Shipped On Time
        
Snap of new calculated column ,

![Snap_1](https://github.com/23Priy/Project--Power-BI/assets/151018390/09e99452-6244-409f-be5f-25d579dbe012)


        
 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;
.  
  
  ### [3] Average Delay 
  
      a) Average delay in arrival(minutes) - 15.09
      b) Average delay in departure(minutes) - 14.71
Average delay will change if different visual filters will be applied.

 ### [4] Some other insights