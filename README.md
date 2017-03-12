Getting and Cleaning Data - Course Project
==========================================

This is the course project repository  for the Data Science's track course "Getting and Cleaning data", available on coursera.org

The dataset being used in this project is: [Human Activity Recognition Using Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

## Files

The code implies that all the data is present in the same folder, un-compressed and without names altered.

- `CodeBook.md` describes the dataset, its variables,  and any transformations or work that was performed to clean it up.

- The R script, `Run_analysis.R`, does the following:
1. Download the dataset if it does not already exist in the working directory
2. Load the activity and feature info
3. Loads both the training and test datasets, keeping only those columns which reflect a mean or standard deviation
4. Loads the activity and subject data for each dataset, and merges those columns with the dataset
5. Merges the two datasets
6. Converts the `activity` and `subject` columns into factors
7. Creates a new dataset that consists of the average (mean) value of each variable for each subject and activity pair.

- `newdataset.txt` is the output of `analysis.R`.
