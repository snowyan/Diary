### Data Wrangling general functions:
* select(): returns a new DataFrame with the selected columns
* filter(): filters rows using the given condition
* where(): is just an alias for filter()
* groupby(): groups the DataFrame using the specified columns, so we can run aggregation on them
* sort(): returns a new DataFrame sorted by the specified column(s).By default the second parameter 'ascending' is True
* dropDuplicates(): returns a new DataFrame with unique rows based on all or just a subset of columns
* withColumn(): returns a new DataFrame by adding a column or replacing the existing column that has the same name. The first parameter is the name of the new column,
  the second is an expression of how to compute it.
