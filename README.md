# Getting-and-Cleaning-Data

## week 3 assignment info:  The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.   The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

# Course Project Assignment

The R script, `run_analysis.R`, produces the following:

1. Loads the activity and feature info
2. Loads both the training & test datasets, keeping only those columns which
   reflect a mean or standard deviation
3. Loads the activity & subject data for each dataset, & merges those
   columns with the dataset
4. Merges the two datasets
5. Converts the `activity` & `subject` columns into factors
6. Creates a tidy dataset that consists of the average (mean) value of each
   variable for each subject & activity pair.

The result can be seen in the file `tidy.txt`.