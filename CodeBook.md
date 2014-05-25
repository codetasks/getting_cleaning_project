##Getting and Cleaning Data project
===================================

This is the CodeBook for run_analysis.R ,part of project in the COURSERA Course " Getting and Cleaning Data " offered by John Hopkins university.

###Script
=======================

This file run_analysis.R contains the script for carrying out the tasks for cleaning and processing the raw datasets available at [https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip] (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)

-Details and description of this data is available at [http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones] (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) [1]

-The data involves data related to Acceleration, Frequency, Jerk, Gyroscope measurements along X,Y,Z Axis, etc the details are available in the features, features_info.txt document available in the dataset folder which can be downloaded from the link provided above. 

**Certain variables that are processed here are **

- mean() - corresponds to Mean value 
- std() - corresponds to Standard deviation
- X, Y , Z - correxpond to the X, Y, Z coordinates
- Subject - subject id in the experiment 
- Label - descriptive label of the activity 
- Types of activity(Levels) - LAYING SITTING STANDING WALKING WALKING_DOWNSTAIRS WALKING_UPSTAIRS

### The whole process here can be categorised into sub-processes.

**-Reading data **

**-Cleaning data **

**-processing data **

**-Data output(write into output files)**


###Tidy data set

**Tidy data set follow certain renaming rules:**

*-No underscores or dots or white spaces or dashes or parentheses*

*-All lower case prefferable *

*-The variable names should be descriptive*

*- No duplications , should be unique*


Functions that are helpful for this task 
gsub()
mean()
sub()
read.table()
write.table()
write.csv()
grep()
colnames()
unique()
names()
cbind()
rbind()



###Patterns that were addressed here 
1. Remove Capital letters
2. Remove dots, parenthesis, white spaces
3. Make variables descriptive ( fullform of abbreviations be preferrably included)
4. Remove duplicates in names like "Body Body" to "body"
5. convert all names to lower case



**Reference:**

*[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012 *
