# MatrixCache
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.  

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

Here are the data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
Goals:

1. You should create one R script called run_analysis.R that does the following. 
2. Merges the training and the test sets to create one data set.
3. Extracts only the measurements on the mean and standard deviation for each measurement. 
4. Uses descriptive activity names to name the activities in the data set
5. Appropriately labels the data set with descriptive variable names. 
6. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.


My program:
run_analysis.R

1. Read subject_train.txt and subject_test.txt files into data tables then binded them into a data table called subject with the column named 'subject'.

2. Read X_train.txt and X_test.txt files into data tables then binded them into a data table called X.

3. Read features.txt into a data table called features.

4. Named the columns of X in by using the the descriptions of the measurements contained in features.

5. Created a data table, called first_data, from X that only contains column names that includes 'std' or 'mean', it is not case sensitive. 

6. Read y_train.txt and y_test.txt files into data tables then bind them into a data table called y with the column named 'activity'.