---
title: "CodeBook"
output: html_document
---


The script run_analysis.R does the following:

### 0.Download the Raw data
Download the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and unzip it

Read the train dataset and test dataset:
x_train: the 561 variables of 7352 subjects.
x_test: the 561 variables of 2947 subjects.
y_train: the activity label of 7352 subjects.
y_test: the activity label of 2947 subjects.
sub_train: the identifier of the subject who carried out the experiment in train dataset (n=7352).
sub_test: the identifier of the subject who carried out the experiment in test dataset (n=2947).

### 1.Merges the training and the test sets to create one data set.
Name the variables in x according the features.txt. 
Give the colname to y and sub.
Merge all the data into dataset.

### 2.Extracts only the measurements on the mean and standard deviation for each measurement.
Extract the colname contain "mean" and "std" from x dataset.

### 3.Uses descriptive activity names to name the activities in the data set
Describe the activity according activity_labels.txt.

### 4.Appropriately labels the data set with descriptive variable names.
Change the colname of dataset according features_info.txt

### 5.From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Group the data according subject and activity, then summary the average.
And save the tidy data as tidy_dataset.txt


