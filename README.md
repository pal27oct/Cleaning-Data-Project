# Cleaning-Data-Project
This contains the project for the Cleaning Data course
Getting and Cleaning Data Course Project
Instructions

You should create one R script called run_analysis.R that does the following:

Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive variable names.
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Links

Data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Data description: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Code book

Variable Subject. 
Subject who performed the activity for each window sample. Its range is from 1 to 30. Sources: subject_test.txt, subject_train.txt
Variable Activity. Activity names. Sources: activity_labels.txt, y_test.txt, y_train.txt (last 2 consists of indicies in 1st document).
Other variables.
Identify measurements. All this columns have exhaustive descriptive names. Sources: features.txt, X_test.txt, X_train.txt (see previous variable description).Script description

Loads and merges test and train sets.
Loads features to name columns, extracts appropriate measurements.
Loads activities indicies, merges it, gets activity labels, adds it to our tidy set.
Loads subject data, merges it, adds it to our tidy set.
Renames column into descriptive names.
Saves tidy set.
Creates new data set with mean of all variables divided by subject and activity.
Saves new set.
