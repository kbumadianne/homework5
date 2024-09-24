# homework5
matplotlib


Final findings from the anti-cancer medication treatment

- Capomulin was a success in reducing tumor sizes in test mice.
- When reviewing tumor sizes in the mice, Capomulin was in the top two drugs to return the smallest tumor size over the course of the treatment
- When compared to the other leading drug, Ramicane, Capomulin had a higher correlation rate between Weight and Tumor Volume. 
- This indicates that when using the correct dosage of Capomulin, the drug will consistently reduce Tumor Volumes within a larger range of weight than Ramicane.



Code Explanation:
Merged the data together and created a new dataframe
Checked for duplicate entries in Mouse ID and Timepoint, filtered on that new dataframe to find the duplicate mice
Once the duplicate mouse was found I created a cleaned dataframe and filtered any dumplicate mice out of the new dataframe
Generated statistics metrics and added them to a pandas dictionary 
Did a more advanced version of the stats summary by grouping by the drug regimen and selecting Tumor Volume to run the stats analysis on
Generated Bar and Pie charts using both Pandas and Pyplot
Found the last timepoint by using the max formula and created a new dataframe
Merged the clean dataframe and the last timepoint dataframe to include the final timepoint
To find quartiles and outliers I started with creating a list of treatment names to refer back to later.  I created an empty list to store Tumor Volume Data
I ran a for loop to iterate over each treatment in the list to get to the tumor volume for that specific drug using loc and append it to the tumor volume list
I create a dictionary for outliers and do a for loop to find the quantiles, do calculations to find the upper and lower bounds.  
I store lower bounds, upper bounds and outliers (using a calculation) to the outlier dictionary.  And use a for loop and f string to print and format the regimen and outlider details
I created a box plot to display the quartiles and outliers
I created a line plot off of a filtered down dataframe
I created a scatter plot off of a filtered down dataframe and averaged weight and tumor volume for each mouse id within the filtered dataframe
I ran a linear regression model and calculated the correlation coefficient to add to the scatter plot
I added a similar scatter plot for a different drug regimen to further analyze the data