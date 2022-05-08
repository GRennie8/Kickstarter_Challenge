# Kickstarting with Excel

## Overview of Project

### How different campaigns fared in relation to their launch dates and funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Firstly I opened the Kickstarter workbook and added a 'Years' column using YEAR() based on the 'Date created conversion'. I created a pivot table to display the 'canceled, failed and successful' results in the columns. 'Parent Category' and 'Years' as filters. 



<img width="447" alt="Pivot_Table" src="https://user-images.githubusercontent.com/104115586/167279423-0a4b4a69-8adc-472d-8ce0-59c2ec1308a4.png">




I filtered 'Parent Category' to theater and changed the row labels to months of the year. The count of outcomes has been sorted in descending order.



<img width="720" alt="Pivot_Table_Filtered" src="https://user-images.githubusercontent.com/104115586/167279436-7153a445-6646-4010-804e-f15e95548fff.png">



Using this data, I created a line graph showing the outcomes based on Launch Date over one year.



![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/104115586/167279450-b625e175-af72-4ebf-94a4-9a63ca845fb8.png)


### Analysis of Outcomes Based on Goals

Using COUNTIFS ()I populated the number of canceled, failed and successful columns 



<img width="817" alt="Formula_1" src="https://user-images.githubusercontent.com/104115586/167279456-1b265a97-cf79-4c95-a53b-c026a506c926.png">



<img width="889" alt="Formula_2" src="https://user-images.githubusercontent.com/104115586/167279458-99259299-f58a-4434-8017-7171d080af9d.png">



<img width="815" alt="Formula_3" src="https://user-images.githubusercontent.com/104115586/167279459-84bcaba7-6c20-44f5-aa06-8661178e57fa.png">



<img width="867" alt="Formula_4" src="https://user-images.githubusercontent.com/104115586/167279461-2db434c6-bbc2-4dec-ade8-7e06f96ef86a.png">



I used =SUM(B2:D2) to populate the 'total projects' column.

=SUM(B2/$E$2) to calculate columns F-H.

This line chart shows the goal amount on the x-axis and the percentage amount on the y-axis.



![Outcomes_vs_Goals](https://user-images.githubusercontent.com/104115586/167279505-4fe98be0-752e-425a-a830-4c57170cd95f.png)




### Challenges and Difficulties Encountered

The main challenge I faced was creating the formula on the 'Outcome Based on Goals' sheet. Specifically the COUNTIFS formula for cells B2:D13. I overcame this difficulty with trial and error until I had a working formula.



## Results

- **What are two conclusions you can draw about the Outcomes based on Launch Date?**

May and June are the 2 months where we can see a high amount of successful kickstarter projects with a 67% and 65% success rate, respectively. October is the month with the most failed projects and a reasonably low number of successful projects. 

- **What can you conclude about the Outcomes based on Goals?**

Generally speaking, the lower the goal, the higher the success rate.

- **What are some limitations of this dataset?**

- **What are some other possible tables and/or graphs that we could create?**

We could include a table comparing the 'average donation' and month to spot any correlation.

