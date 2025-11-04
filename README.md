
☔️ Python Data Analysis Project Weather Dataset Analysis

🎯 Project Scope and Goals

This project represents a practical application of Big Data analysis using Python We focused on analyzing a realworld Weather Dataset to extract specific meteorological information The project successfully addressed a set of 15 defined questions using advanced Python and data analysis commands

📊 Dataset Specifications

The data used for this analysis is the Weather Dataset which was provided in CSV file format

The dataset contains a significant amount of information
Total Records Rows 8784
Total Columns 8

The original columns tracked various conditions including Date Time Temperature Dew Point Temperature Relative Humidity Wind Speed Visibility Pressure and the weather Condition originally named Weather

Note on Data Types Initial exploration using dtypes showed that the Date Time column was an Object data type and would need conversion for proper analysis

🛠 Required Tools and Libraries

The core technology stack for this analysis includes
Python
The Pandas library was imported to handle data manipulation

Key Analysis Functions and Techniques

The following functions and methods along with logical operators were crucial in solving the 15 analytical questions

🔎 Data Exploration and Structure Checks

head Displays the first number of rows defaulting to 5 of the DataFrame
shape Outputs the total number of rows 8784 and columns 8
index Shows the index attributes of the DataFrame starting from 0 and running up to position 8783
columns Lists all the names of the columns within the dataset
dtypes info Displays the data type of each column and provides basic information including the index range and memory usage eg 5490 KB

🧹 Data Cleaning and Integrity

isnull notnull Used to check for the presence of Null missing values across the dataset The analysis confirmed there were no single Null values present
rename Used to change the column name permanently The column originally named Weather was renamed to Weather Condition using the inplaceTrue argument

🧮 Unique Values and Frequency

unique Essential for viewing all distinct elements present within a specific column eg finding all unique Wind Speed values
nunique Calculates the total count of unique values present in a column or across the whole DataFrame
valuecounts Shows the count frequency of each unique element in a column eg Clear weather appeared 1326 times and Snow appeared 390 times

📉 Statistical Calculations

These functions were applied specifically to numeric columns like Relative Humidity and Pressure
mean Used to find the average mean value of a column eg mean Relative Humidity
std Used to calculate the Standard Deviation eg calculating 08444 for the Pressure column
var Used to calculate the Variance eg variance of Relative Humidity was found to be 28672
min and max Used in conjunction with grouping to determine the lowest and highest values of numerical metrics against unique weather conditions

🎯 Filtering and Conditional Analysis

Filtering Boolean Masking This technique was used to select records that met a specific requirement such as finding the 474 records where the Wind Speed was exactly 4 kmh
String Containment strcontains This vital command was used to find all records where a column like Weather Condition contained a specific word like Snow regardless of whether it was a full or partial match eg Snow or Freezing Snow
Logical Operators
AND Operator Used to filter records that must satisfy two or more conditions simultaneously eg Wind Speed 24 AND Visibility 25
OR Operator Used to filter records that satisfy at least one of multiple conditions eg Weather is Clear OR Visibility 40
Grouping groupby This function was used to perform analytical operations like mean min max on all other columns segmented by the unique values of the Weather Condition column

