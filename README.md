# surfs_up
## Challenge

The premise for this analysis was to determine whether or not there would be a seasonal aspect to our ice cream sales based on comparison of weather data from June and December.

We used sqlalchemy to gather the data for June only and December only from our database.

Then, we used Pandas to manipulate the data for comparison.

Here is the key statistical data for precipitation for both June and December for years 2010-2017:

<img src="https://github.com/songmanrob/surfs_up/blob/master/prcp_df_describe.png" width="25%" height="25%">

As shown above, the quartiles are fairly similar between the two. The average(mean) precipitation for December is nearly 1/10 inch higher and the max precipitation is higher, but since the quartiles are so close, the overall effect on the ice cream sales will probably be negligible.

The boxplot y-axis had to be limited to under 1/2 inch just to see the statistical difference between the two. That's a pretty good sign.

<img src="https://github.com/songmanrob/surfs_up/blob/master/prcp_df_boxplot.png" width="50%" height="50%">


Here is the key statistical data for temperature for both June and December for 2010-2017:

<img src="https://github.com/songmanrob/surfs_up/blob/master/temp_df_describe.png" width="25%" height="25%">

Again, we see that the stats are very similar. December can be a bit cooler at times, but overall, it's still very temperate and great ice cream weather.

<img src="https://github.com/songmanrob/surfs_up/blob/master/temp_df_boxplot.png" width="50%" height="50%">


We could deepen this analysis by generating these comparisons separately for each reporting station and then analyze the reliability of each station to make sure that our data is the best it can be.

Also, for further analysis, we could investigate the number of days of significant precipitation in each month to get an idea of how many days we are likely to be "rained out" of sales for each month. We could then do the same for temperature, figuring how many days it is too cold for ice cream (if such a thing exists).


In conclusion, based on the data we've gathered to this point, there doesn't seem to much significant difference in precipitation or temperature between June and December which is great news for ice cream sales all year long!
