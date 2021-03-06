### CodeBook

Describes the variables, the data, and any transformations or work to clean up the data called


## The Data

This project uses data from the Human Activity Recognition Using Smartphones Data Set. It can be found [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).

From the source:
* The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. 
* Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. 
* Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. 
* The experiments have been video-recorded to label the data manually. 
* The obtained dataset has been randomly partitioned into two sets, the training data and the test data.
* The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). 
* The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. 

## The Variables

run_analysis.R imports the train data from '/train/X_train.txt', '/train/y_train.txt', and '/train/subject_train.txt' into x_train, y_train, and subject_train respectively. 
It imports the test data from '/test/X_test.txt', '/test/y_test.txt', and '/test/subject_test.txt' into x_test, y_test, and subject_test respectively. 
The activity labels are imported from '/activity_labels.txt' into activities, and the names of the measurements are imported from '/features.txt' into features.
The Transformations

run_analysis.R does the following:

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
