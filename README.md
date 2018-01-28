# DAND - Create a Tableau Story

Workbook links:
1st attempt: https://public.tableau.com/profile/raahul4197#!/vizhome/TitanicWorkbook1/TitanicSurvival
Final attempt: https://public.tableau.com/profile/raahul4197#!/vizhome/TitanicWorkbook2/TitanicSurvivalv2

Data:
I used `titanic-data.xlsx`, which is derived from `titanic-data.csv`, because Tableau was having trouble importing the csv file. But they're equivalent.

## Summary
The dataset consists of demographics and passenger information for a subset (891) of the 2224 passengers on boar the Titanic. We visualize the various demographical aspects of a passenger that are correlated to his/her survival. We gain insight into what kind of passengers survived the most, and what kind of passengers survived the least, and what contributed to this.

## Design
1. For the first slide, I wanted to visualize the survival of passengers in every age group. I had divided the age group in intervals of 10 years. After getting some feedback, I turned this into interval of 20 years, which showed the trend better.

1. Since age played a big role in survival, I wanted to facet all the other variables in terms of age, so that the combined influence could be visualized better. I decided to show the survival by gender and age. To clearly show the constrast between males and females surviving, I also pulled in a bubble chart, so that comparing the relative sizes of genders who survived woud give the viewer a clear idea of the trend.

1. I also incorporated gender into showing the survival for each class of the ticket. However, the bar plot became very confusing to understand, and was monotonous since there were a lot of bar plots already in the story. So, I removed this plot from the 2nd slide and only kept it in the 3rd slide. I also turned it into a faceted bubble chart, because it became much easier to draw comparisons between both gender, as well as the ticket class.

1. For showing the survival of people against the number of family members (no. of parents/childrens or siblings/spouse), I used a line chart to emphasise the downward trend. The more family members you had with you, the less chances of survival.

## Feedback
I received the following feedback:

1. In the very first slide, where we see a histogram of passenger age and no. of passengers who survived, I initially grouped age into buckets of 10 years. However, I got a feedback that this is hard to read. A much better approach would have to group them into 20 years, so that the larger trend is visible.

1. This was more of a mistake on my part. The survival by gender and age had a couple of problems. First, since it was rendered as a bar graph instead of a histogram, the x axis labels (0, 10, 20, etc.) did not look good, because age groups are ranges, not an absolute value. It was fine to have the grouping as 10 years though. Also, the labels for the counts on the bar graph were wrong, because they printed the actual age group rather than the count. Also, on hovering, instead of saying "No. of passengers", it said "Count of age", which was confusing.

1. On the second slide, survival of gender vs. ticket class, the bar graph looked very monotonous and repetitive. I was suggested to use a bubble chart, where size was the "percentage" of people who survived, and class were separate bubbles. Also, I could color code them by gender. Since I used the same graph in slide 3, I was suggested to add something else instead.

## Resources
Udacity videos and Tableau documentation and tutorials.
