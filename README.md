# Health-Scores-and-Food-Poisoning
This repository contains the source files, class files, and .jar files developed for the PBDAA Spring 2023 Final Project.

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


# Inspection Profiling
All Java source files, .class files, and .jar files developed to clean the original Health Inspection data are included in the Inspection Cleaning folder. The data is cleaned through process of Hadoop MapReduce.
