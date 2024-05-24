# Executive Summary- Finance Report


## Problem Statement

This dashboard helps the airlines understand their customers better. It helps the airlines know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average delay & departure time, thus since by using this dashboard they have identified this problem, they can further work on factors responsible for these unwanted delays.

Since, number of neutral/dissatisfied customers (almost 57 %) are more than satisfied customers (around 43 %), thus in all they must work on improving their services. 

Also since average delay in arrival & departure both is 15 minutes, thus they must try to reduce it.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a Excel file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : In the report view, under the view tab, theme was selected.
- Step 5 : Since the data contains various ratings, thus in order to represent ratings, a new visual was added using the three ellipses in the visualizations pane in report view. 
- Step 6 : Visual filters (Slicers) were added for  fields named Date.
- Step 7 : Map, stacked column chart and chart Line  visuals were added to the canvas, one representing Profit by Country & other representing profit by Date & other Representing unit sold and prduct sales by segment.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
  
  
In our dataset, Some parameters were assigned value 0, representing those parameters are not applicable for some Products and unit sales.

All these values have been ignored while calculating average rating for each of the parameters mentioned above.

- Step 8 : In the report view, under the insert tab, two text boxes were added to the canvas, in one of them name of the airlines was mentioned & in the other one company's tagline was written.
- Step 9 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted & similarly using image option company's logo was added to the report design area. 
- Step 10 : Calculated column was created in which, customers were grouped into various age groups.

for creating new column following DAX expression was written;
       
    
        
Snap of new calculated column ,

        
- Step 15 : New measure was created to find total count of customers.

Following DAX expression was written for the same,
        
        Count of unit_sold = COUNT(financial[units_sold])
        
 - Step 16 : New measure was created to find  % of customers,
 
 Following DAX expression was written to find % of customers,
 
         Total_sales = SUM(financial[sales])
 
 # Report Snapshot (Power BI DESKTOP)
- power report file uploaded
 
