1. Use the pandas library to import an input CSV file, which creates a data frame from the data.
2. Changed the data type of all date columns from object to datetime.
3. Removed the dates from each employee's row and arranged them in chronological order.
4. Made an empty data frame with relevant variables in it.
5. I've used an if condition statement-nested for loop to insert values to this empty data frame.
6. The dates are iterated over in the first two for loops. The third for loop iterates through the original dataframe's rows. Since our data is of series data type, I extracted the column names in the third for loop by using (.index). In series data type column names are designated as indexes.
7. If my date of joining equals effective date, then add values to the data, assuming that my date of joining is the smallest date in relation to other dates. i+1 since Python's range begins at 0 and repeated the process for the remaining columns.
8. Since I needed the end date to be one day before of the next effective date, I used the timedelta function in the datetime library to obtain the end date column.
9. As required, we had to assign latest employees date of exit as far future date (01-01-2100) the following is achieved using for loop.
