# Getting-and-Cleaning-Data-Course-Project
Week 4 assignment for peer rivew
This assignment was done to learn cleaning data. The data linked from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones Here are the data for the project:https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

1.  "run_analysis.R" contains all the code to perform the analyses described in the 5 steps below. They can be launched in RStudio by just importing the file.For the code to work , the data has to be in the same folder in zipped form.

2. Steps performed on data:
#loading file from URL# the Url has zipped file, thus unzip the file#There are multiple files in the folder thus to know the list of files, thus get to know the files# After reading README file as instructed in the assignment# we understand that there is test and train data having variables whose names are listed in features file# performing certain activity# performed by certain subjects# now read data into variables from file 
#1. Merge training and test data set to create one data set## adding rows at end to get merged data set## adding meaningful names to variables## merging whole data sets
#2.Extracts only the measurements on the mean and standard deviation for each measurement.# After few trials and reading i understood the meanfrequency has to be excluded thus the "()"
#3.Uses descriptive activity names to name the activities in the data set
#4.Appropriately labels the data set with descriptive variable names
#5.From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

2. tidydata.txt contains the output of the code "run_analysis.R".

3. The variables  means the following:
filesinfolder - has list of files in zipped folderdata
ActivityTest, dataActivityTrain, dataSubjectTest, dataSubjectTrain, dataFeaturesTest, dataFeaturesTrain - raw data
dataSubject, dataActivity, dataFeatures - merged data for subject, activity, features
dataFeaturesNames - has names of features
dataMerged - has merged data 
setMeanStdNames - has names from dataFeaturesNames which are required
dataMergedlater - has data for MeanStdNames variables from dataMerged
dataMergedlater1 - has tidy data post calculating mean 
tidydata.txt - has the output
