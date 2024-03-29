# Power BI - Data Visualization

## Data Used
Data used to make the report is added to the file section named "Sample Superstore" which is a .xlsx file.
## Problem Statement

The report that was prepared  initially in Tableau and had to be migrated/reflect it into Power BI. I studied the report as to what visuals are used , DAX used to create calculated columns and measures and prepared the same report in Power BI.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a .xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options to check for any error or empty data values. 
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Visual filters (Slicers) were added as needed on every Page.
- Step 7 : 5 Pages made are :- Executive view, Customer analysis, Shipping Analysis, Order Sumamary And Sales forecast.
- Step 8 : To calculate Profit ratio, Shipping time and various other needed columns DAX is used in power bi desktop. 
- Step 9 : I tried to stick to what the motive of the Project was and therefore used the same visuals to show the data .
  

  

for creating new column following DAX expression was written;
       
        order days = ABS(Merge1[Ship Date]- Merge1[Order Date])
        Shipment Time = IF(Merge1[order days]>3,"Shipped Late") & IF(Merge1[order days]<3,"Shipped Early") & IF(Merge1[order days]=3,"Shipped On Time
        Profit ratio = DIVIDE('Orders (3)'[Profit],'Orders (3)'[Sales])
        
Snap of new calculated column ,

![Snap_1](https://github.com/23Priy/Project--Power-BI/assets/151018390/09e99452-6244-409f-be5f-25d579dbe012)
![Snap_2](https://github.com/23Priy/Project--Power-BI/assets/151018390/afa200c6-0402-4075-8707-cd65ef90925f)


        
 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://github.com/23Priy/Project--Power-BI/assets/151018390/9873aac3-0c29-4ec5-ba6b-7ef7b794c960)
![Dashboard_upload](https://github.com/23Priy/Project--Power-BI/assets/151018390/dae8b5e7-5af9-4a0e-a81d-d5aa2582cfaf)
![Dashboard_upload](https://github.com/23Priy/Project--Power-BI/assets/151018390/18dc8cfc-f88b-401f-8324-1672a9a1299b)
![Dashboard_upload](https://github.com/23Priy/Project--Power-BI/assets/151018390/fc2e8346-5703-4d21-b307-bcda5f2f1843)
![Dashboard_upload](https://github.com/23Priy/Project--Power-BI/assets/151018390/ad355014-d6e4-4d14-acc7-2ed603938301)
 

Outcomes Achieved

This was my first project report, I made in Power BI after completing Power BI training. Tt was just to practice my skills in a practical problem so that I learn from my mistakes and uncover my depth of knowledge of the tool which i did and was a good experience to do so. 
