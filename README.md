# Linear-Regression-for-College-ROI
I explored the question on which factors is more important to return of invesment for college students.

Some difficultries i had making this project:
1. I didn't know that making a column based wholly on another column as in the case for df["student_was_active"] was the primary source on how we calculated df["stem_active"] and df["non-stem_active"]. Therefore, i needed to drop both columns before making a linear regression model
2. The most tricky part of this project by far is to analyze a data which have a lot of 0 or na values since the query was so specifi. I decided to use the describe function which bypass all of the NaN values which i have.
3. Another difficulty i had was to understand the errors i had in making the summary for the regression linear table. Turns out, i figured out later that i needed to convert those summary to pandas dataframe then change the decimal for the dataframe.

For the results i had this is how to read it:
1.  81,870 corr = institution_tier had the biggest significance which means for 1 addition to the instituion tier it effects the ROI as much as $81,870.0
2.  71,750 corr = major_category had the second biggest significance which means for 1 addition to the instituion tier it effects the ROI as much as $71,750.0
3.  46 450 corr = had_internship is third for significance which means for 1 addition to the instituion tier it effects the ROI as much as $46,450.0
4.  29,490 corr = student_was_active is fourth for significance which means for 1 addition to the instituion tier it effects the ROI as much as $29,490.0

*note
the GPA variable is noted as having a negative correlation but this is caused by the competing variables that are fighting for significance. And not because it does not have positive significance
