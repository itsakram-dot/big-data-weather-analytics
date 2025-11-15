# Big Data Weather Analytics

This project demonstrates how to process **NCDC weather station data** using **Hadoop**, **PySpark**, and **mrjob**. The assignment is divided into four parts, each focusing on a different big-data concept such as MapReduce, Spark RDD transformations, and Hive/Pig queries.

---

## Project Contents

1. **MedianTemp_MRjob.py**  
   - *Part 1*: Computes the median wind direction per month from NCDC records using mrjob (Mapper/Reducer in a single Python file).

2. **RangeWeather.py**  
   - *Part 2*: PySpark application calculating the **range** (max-min) of visibility distance for each weather station.

3. **Ques3.py**  
   - *Part 3*: Another mrjob script retrieving USAF weather station IDs and visibility distances, writing them to a text file for further processing.

4. **annotated-output1.txt** (or `.pdf`)  
   - Sample output showing station IDs and visibility values from Part 3.

5. **CourseProject_fall2024.docx**  
   - Original assignment instructions detailing how each part should be implemented and tested.

---

## How to Run

Part 1: Median Wind Direction (mrjob)
python MedianTemp_MRjob.py --input /projectdata --output /path/to/output

Part 2: Visibility Range (PySpark)
spark-submit RangeWeather.py

Part 3: Station ID & Visibility Data
python Ques3.py --input /path/to/projectdata --output /path/to/output

Part 4: Pig & Hive
pig -x local pig_script.pig
hive -f hive_script.sql






   
