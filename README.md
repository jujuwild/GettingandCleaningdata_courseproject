### Getting and Cleaning Data Course Project
## Motivation of Data Set

This data set is motivated by the course project of Getting and Cleaning Data  week4 from Coursera John Hopkins University Data Science Special Section. 
The purpose of the project is to obtain a tidy dataset from a raw data set. The original data set is obtained from the [Human Activity Recognition Using Smartphones Data Set](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) in UCI Machine Learning Repository.


For the smartphone data set, relevant experiments were carried out with a group of 30 volunteers within an age bracket of 19-48 years old. 
Each individual performed six different activities wearing a smartphone, including walking, walking upstairs, walking downstairs, sitting, standing and laying. The smartphone had an embedded accelerometer and gyroscope to capture the movement of the individuals.

# This repository includes the following files

* README.md: explains the scripts and how they are connected

* FinalData.txt: a tidy data set with unique identifiers subject and activity

* run_analysis.R: code generating the tidy data set from raw data recorded in the Human Activity Recognition Using Smartphones Data Set. The process of generating a  tidy data set includes the following steps:
1. Merges the training and the test sets to create one data set called Merged_Data.
2. Extracts only the measurements on the mean and standard deviation for each measurement to get TidyData.
3. Uses descriptive activity names to name the activities in the data set.
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject FinalData.

* CodeBook.md: a code book that describes the variables, the data and tranformations

