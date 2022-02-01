### Data Wrangling general functions:
* select(): returns a new DataFrame with the selected columns
* filter(): filters rows using the given condition
* where(): is just an alias for filter()
* groupby(): groups the DataFrame using the specified columns, so we can run aggregation on them
* sort(): returns a new DataFrame sorted by the specified column(s).By default the second parameter 'ascending' is True
* dropDuplicates(): returns a new DataFrame with unique rows based on all or just a subset of columns
* withColumn(): returns a new DataFrame by adding a column or replacing the existing column that has the same name. The first parameter is the name of the new column,
  the second is an expression of how to compute it.
  
![Spark Eco System](/sparkecosystem.png "Spark Eco System")

### 03 Spark RDD
* Need for RDDS
* What are RDDs
* Features of RDDS
* Creation of RDDS using spark
*  three types to create the rdds 
   1: spark.sparkContext.parallelize() or sc.parallelize()
   2: spark.read.textFile() 
   3: use transformation to create a new rdd
* Operations performed on RDDS
  1: Transformations -- Narrow Transformations (map(), filter(), flatMap(), partition(), mappartition())and Wide Transformations(reduceBy(), Union())
  
  2: Actions -- collect(), count(), take(), First()
