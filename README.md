# Movie Genre Analysis using Spark Pair RDDs
## Apache Spark RDD Project
A PySpark project using Pair RDDs to analyze movie genres, perform distributed aggregations, and extract insights from a large dataset.

## Objective
This project uses Apache Spark Pair RDDs to analyze a movie dataset and extract insights about genre distribution.

## Dataset
The dataset used is `movies.csv`, which contains:
- movieId
- title
- genres

## Technologies Used
- Python
- PySpark
- Apache Spark (RDD API)

## Key Operations Performed
- Created Pair RDDs from the movie dataset
- Used `flatMap()` to split movies into multiple genre pairs
- Applied `reduceByKey()` to count movies in each genre
- Used `lookup()` to retrieve movie titles for a selected genre
- Used `groupByKey()` to group movies by genre
- Used `countByKey()` to count records by key
- Applied caching for performance optimization

## Key Insights
- Drama is the most common genre
- Comedy is also highly represented
- Some genres like IMAX are rare
- A movie can belong to multiple genres

## Learning Outcomes
- Pair RDD transformations and actions
- Difference between `reduceByKey()` and `countByKey()`
- Use of `lookup()` and `groupByKey()`
- Lazy evaluation and caching in Spark
