# Week-11

Update Week 11:
-Known issue: displaying the data into different rows is still being an issue, as I chose to focus on the technical details of having the data and calculations working inside the table instead. I was able to get the data in each row initially, but since my array is comprised of 43 different arrays, it displays the results in a very strange way so I decided to leave the final result in the first row instead.
-Calculations inside the table: this was solved by using a for in loop and doing the calculations while the loop is active, as the data wasn't already available inside the table.
To-Do:
-Solving the display to different rows, which will also solve the display of the trend arrows, as those are only contained in the first cell of their column, and don't really match the font size of the rest of the data. Will try to solve this using a reduce function...
-Sorting all the data together, using the sort function for all the columns at once - I can't do this until the data is displayed in different rows.


ReadMe From Week 10:
I had to scale down the matrix to only show a few indicators from the OECD page, instead of adding some scoring based on the results of each value. The matrix may still contain a column with variations of unemployment from one year to another, based on the inputs obtained for the different years with the API.

To Do List: 
-Getting the data from the API is successfully done, but the data obtained doesn't really display in their own row yet. The reason is, the array created from the values obtained via the API seem to be a single object containing 43 different single arrays (instead of a single array containing 43 values). I will have to find a way how to merge all of those into one single array, so I can distribute the values in the table properly. So far, when using a for loop function to distribute the array into the html table, each array of value has only one item (0), so the loop takes a single letter is distributed into a single cell...instead of a country name or value, distributed into a single cell. 
-Getting the rest of the API data (rates for 2016 at least, not sure 2018 has been released yet) - this should be quite easy to do, as the logic should be exactly similar to what I've done for the year 2017. 
-Adding calculations to the variations row. This could be tricky, as I'm not sure how to input calculations in html, when there is no table already created (all the rows are getting added, as the API return the values from the OECD site). 
-Sorting data: I still don't have my array working, so I can't quite sort the data yet. -Formatting the table better, and html page.
