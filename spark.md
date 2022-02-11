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
  * RDD is the heart of Apache spark
* Features of RDDS
* Creation of RDDS using spark
*  three types to create the rdds 
   1: spark.sparkContext.parallelize() or sc.parallelize()
   2: spark.read.textFile() 
   3: use transformation to create a new rdd
* Operations performed on RDDS
  1: Transformations -- Narrow Transformations (map(), filter(), flatMap(), partition(), mappartition())and Wide Transformations(reduceBy(), Union())
  
  2: Actions -- collect(), count(), take(), First()
### 04
### 05 Spark SQL
* Why Spark SQL
* Spark SQL libraries
* Spark SQL Features
  * SQL Integration with Spark
  * Uniform Data Access
  * Seamless Support
  * Transformations
  * Performance
  * Standard Connectivity
  * User Defined Functions
* Hands-on Examples
* Stock Market Use Case
* How to use SQL
  * import org.apache.spark.sql.SparkSession
  * import spark.implicits
  * val df = spark.read.json()
  * df.show(), df.select("name").show(); df.select($"name", $"age"+1).show()
  * Adding Schema - Reading File and Adding Schema
  * Json data
    -- how to create Json file?
  * Hive tabels - Case class and Spark Session
  * Hive Tables -- SQL & DataFrame Transformation
  * Hive Tables -- Result
* Use case --Stock Market trading
  * The Requirements: 1, Process huge data 2, Handle input from multiple sources 3, Process data in real-time 4, Easy to use and not very complex
  * Implementing Stock Analysis Using Spark SQL
* Running SQL Queries
  * Register the DataFrame as a SQL temporary view (df.createOrReplaceTempView("people")
 
