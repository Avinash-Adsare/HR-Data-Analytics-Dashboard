

# HR Analytics

## Problem Statement:

The HR Director of a company has recently noticed an increase in employees leaving (attrition). She would like to figure out any trends or patterns. She has surveyed the staff and provided you with the data.

She would like to know what the attrition rate is (% of people who have left).

She would also like to know if factors like age, years at the company and income play a part in determining if people will leave or not.


## Lessons

### Loading the dataset

Data is available in CSV Format. Just Click on the Text/CSV on the Landing page in the data source section. Search for the path and just load the data.


### Sheet 1 - AgeWise Employee count:

Firstly, Create a new column age(groups) by taking the age column and grouping them into 5 age groups namely-
18-25, 26-35, 36-45, 46-55, 56-60.

Then Create a stacked barchart showing employee count by age group. To show attrition, click and drag the attrition column to colors in the Marks Shelf.

Rows : Age(group)

Columns: Employee Count (sum)

### Sheet 2- Average Monthly Income by age:

Dual barchart showing average monthly income by age group and another chart showing how much each age group is earning based on the average income of the whole company.

Firstly, Create a level of detal expression (LOD), for this create a calculated field for average per age group and write the following formula
{fixed [Age (group)] : AVG([Monthly Income])}

Now create another LOD expression by creating a calculated field and using the following formula
{fixed : AVG([Monthly Income])}

Now create a calculated field to show Amount from age group using formula
SUM([Total Average])-SUM([Avg per age group])

Rows : Average per age group(sum) and Amount from group average(average)

Columns :  Age(group)

### Sheet 3 - Employee Count by Income:

A Simple Histogram Showing Monthly Income by bin size of 2000. To show attrition, click and drag the attrition column to colors in the Marks Shelf.

Rows : Monthly imcome (Count)

Columns : Bin(Monthly imcome) - Autogenerated when you click on the histogram chart

### Sheet 4 - Employee count by Experience:

A Barchart showing Employee count by years worked at company. To show attrition, click and drag the attrition column to colors in the Marks Shelf.

Rows : Employee Count (sum)

Columns : Years at Company


### Headline cards:

        Total Employee Count: Show Employee Count as a text box

        Employee Leaving Rate: Use Calculated Field to create Attrition Employee Count using formula 
                IF  [Attrition] = "Yes" THEN  [Employee Count] ELSE 0 END
        Then create a calculated field for attrition rate using formula
                sum([Attrition Employee Count])/sum([Employee Count])

            Show Attrition rate as text box

        Job Satisfaction: Show Job satisfaction (Average) as a text box

        Average Monthly Income: Show Monthly Income (Average) as a text box

### Dashboard:

Dashboard Size : 1300 x 900

I have used Horizontal and vertical objects to place various sheets. Just drag and drop the sheets and adjust the sizes as per your conveinence.

Filter : Made on Attrition and apply it to apply on all the worksheets.

Click on use as a filter for all the visuailzation to show customized visuals 

Use text object to write the heading.