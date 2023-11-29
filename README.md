# Health-Scores-and-Food-Poisoning
This repository contains the source files, class files, and .jar files for a project analyzing the relationship between restaurant health scores and food poisoning cases reported by NYC OpenData. 

# Original Data
The original datasets downloaded from NYC OpenData can be found in the Original Data folder. These are both the food poisoning and health inspection datasets.

# Food Poisoning Cleaning
All Java source files, .class files, and .jar files developed to clean the original Food Poisoning data are included in the Food Poisoning Cleaning folder. The data is cleaned through process of Hadoop MapReduce. Cleaning yields the following schema:
* Reported Date - String
* Zip Code - String
* Borough - String - {Manhattan, Brooklyn, Bronx, Queens, Staten Island}
* Latitude - Float
* Longitude - Float


# Inspection Cleaning
All Java source files, .class files, and .jar files developed to clean the original Health Inspection data are included in the Inspection Cleaning folder. The data is cleaned through process of Hadoop MapReduce. Cleaning yields the following schema:
* Borough - String - {Manhattan, Brooklyn, Bronx, Queens, Staten Island}
* Zip Code - String
* Inspection Date - String
* Critical Flag - String - {Critical, Not Critical, Not Applicable}
* Score - Integer 
* Grade - Character - {A, B, C, N}
* Latitude - Float
* Longitude - Float
* Health Score Above 17 - Integer - {0, 1}
Cleaning decreases the size of the data from 206149 rows to 104265 rows.

# Inspection Profiling
All Java source files, .class files, and .jar files developed to profile the original Health Inspection data are included in the Inspection Cleaning folder. The data is profiled through process of Hadoop MapReduce. Ultimately profiling yields critical counts, unique grade gounts, unique borough counts, and a total unique zipcode count.

# Food Poisoning Profiling, Merging Datasets and Final Analytic Code
main.scala is a scala file that profiles the Food Poisoning dataset, merges the two cleaned datasets, and ultimately conducts our analytic by utilizing Pearson correlation coefficient testing and calculations as well as multinomial logistic regression analysis.


