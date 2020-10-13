# Human_Capital_Analytics
## Exploration of HR Analytic Data of a fictions small company

### Introduction
The following synopsis was provided by Dr. Rich Hubber who published the data on kaggle.  

The HR Dataset was designed by Drs. Rich Huebner and Carla Patalano to accompany a case study designed for graduate HR students studying HR metrics, measurement, and analytics. The students use Tableau data visualization software to uncover insights about the case. This is a synthetic data set created specifically to go along with the case study (proprietary for the college that we teach at).

Every year or so, we update the data set to include additional columns, and to make slight changes to the underlying data. In this version, we add several new features to the data set:

Engagement Survey Results, a floating-point number, range between 1 and 5.
Special Project Count, integer, which is the number of special projects the employee worked on in the last year.
Last Performance Review Date, date, to ensure that all employees are receiving timely reviews.
Days Late in the Last 30 days, integer, as an attendance metric.


### Data Source
https://www.kaggle.com/rhuebner/human-resources-data-set?select=HRDataset_v13.csv

### Feature Dictionary

![](dictionary.png)

### NOTE: To view jupyter notebook html based content fully rendered, please use the nbviewer link:
https://nbviewer.jupyter.org/github/Vajrasamaya/Human_Capital_Analytics/tree/master/


## Visualizations

### Based on Sex

![](Images/Mean_Performance_Sex.png)

![](Images/Employee_Count_Sex.png)
Not only are mean performance scores higher for women, but women constitute a majority of employees.

![](Images/Mean_Rate_of_Pay_Sex.png)
And yet, despite better performance reviews for women, and despite the fact that more employees in the company are women, higher pay is awarded to men.


### Based on Racial Description
![](Images/Employee_Satisfaction_Race.png)

![](Images/Employee_Engagement_Race.png)


![](Images/Mean_Performance_Race.png)
Surprisingly, Performance scores for native americans are signifantly higher that any other racial category.  This is especially peculiar because the mean performance score range for the rest of the racial groups is .25 whereas the mean performance score for Native americans is .5 higher than the next group, white employees.  There doesn't appear to be a reason for this except for the presence of an outlier. So I look at employee counts by race.

![](Images/Employee_Count_Race.png)
When we review the counts, the story told is quite different.  Here we can see that there simply are very few native Americans who are employees, totalling four.  By contrast, there are 193 White employees and 57 black employees. Consequently, the mean score for native Americans is affected to a far greater extent by an individual employees score than is a member of other groups.  

What might this mean?  It's hard to say.  My first thought was that this was a significant indicator of discriminatory hiring practices because the company has employees in 28 states.  However, by looking at employee counts by state, we can see an overwhelming concentration of employees in one state; this might indicate that the distribution of employees by race is simply a result of of the demographics of that state.

![](Employee_Count_State.png)

![](Images/Mean_Pay_Race.png)
