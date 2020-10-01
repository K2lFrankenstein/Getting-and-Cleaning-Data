### Script Name: 'run_analysis.R'

### Source: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones    

## Identifiers
- Subject Number - The ID number of the test subject (1-30)
- Activities - The types of activities performed when the measurements were taken (1-6)


## Features 
### (all measurements were normalized from -1 to 1)
- timeBodyAccelerator Mean-X
- timeBodyAccelerator Mean-Y
- timeBodyAccelerator Mean-Z
- timeBodyAccelerator Standard Deviation-X
- timeBodyAccelerator Standard Deviation-Y
- timeBodyAccelerator Standard Deviation-Z
- timeGravityAccelerator Mean-X
- timeGravityAccelerator Mean-Y
- timeGravityAccelerator Mean-Z
- timeGravityAccelerator Standard Deviation-X
- timeGravityAccelerator Standard Deviation-Y
- timeGravityAccelerator Standard Deviation-Z
- timeBodyAcceleratorJerk Mean-X
- timeBodyAcceleratorJerk Mean-Y
- timeBodyAcceleratorJerk Mean-Z
- timeBodyAcceleratorJerk Standard Deviation-X
- timeBodyAcceleratorJerk Standard Deviation-Y
- timeBodyAcceleratorJerk Standard Deviation-Z
- timeBodyGyroscope Mean-X
- timeBodyGyroscope Mean-Y
- timeBodyGyroscope Mean-Z
- timeBodyGyroscope Standard Deviation-X
- timeBodyGyroscope Standard Deviation-Y
- timeBodyGyroscope Standard Deviation-Z
- timeBodyGyroscopeJerk Mean-X
- timeBodyGyroscopeJerk Mean-Y
- timeBodyGyroscopeJerk Mean-Z
- timeBodyGyroscopeJerk Standard Deviation-X
- timeBodyGyroscopeJerk Standard Deviation-Y
- timeBodyGyroscopeJerk Standard Deviation-Z
- timeBodyAcceleratorMagnitude Mean
- timeBodyAcceleratorMagnitude Standard Deviation
- timeGravityAcceleratorMagnitude Mean
- timeGravityAcceleratorMagnitude Standard Deviation
- timeBodyAcceleratorJerkMagnitude Mean
- timeBodyAcceleratorJerkMagnitude Standard Deviation
- timeBodyGyroscopeMagnitude Mean
- timeBodyGyroscopeMagnitude Standard Deviation
- timeBodyGyroscopeJerkMagnitude Mean
- timeBodyGyroscopeJerkMagnitude Standard Deviation
- frequencyBodyAccelerator Mean-X
- frequencyBodyAccelerator Mean-Y
- frequencyBodyAccelerator Mean-Z
- frequencyBodyAccelerator Standard Deviation-X
- frequencyBodyAccelerator Standard Deviation-Y
- frequencyBodyAccelerator Standard Deviation-Z
- frequencyBodyAccelerator MeanFreq-X
- frequencyBodyAccelerator MeanFreq-Y
- frequencyBodyAccelerator MeanFreq-Z
- frequencyBodyAcceleratorJerk Mean-X
- frequencyBodyAcceleratorJerk Mean-Y
- frequencyBodyAcceleratorJerk Mean-Z
- frequencyBodyAcceleratorJerk Standard Deviation-X
- frequencyBodyAcceleratorJerk Standard Deviation-Y
- frequencyBodyAcceleratorJerk Standard Deviation-Z
- frequencyBodyAcceleratorJerk MeanFreq-X
- frequencyBodyAcceleratorJerk MeanFreq-Y
- frequencyBodyAcceleratorJerk MeanFreq-Z
- frequencyBodyGyroscope Mean-X
- frequencyBodyGyroscope Mean-Y
- frequencyBodyGyroscope Mean-Z
- frequencyBodyGyroscope Standard Deviation-X
- frequencyBodyGyroscope Standard Deviation-Y
- frequencyBodyGyroscope Standard Deviation-Z
- frequencyBodyGyroscope MeanFreq-X
- frequencyBodyGyroscope MeanFreq-Y
- frequencyBodyGyroscope MeanFreq-Z
- frequencyBodyAcceleratorMagnitude Mean
- frequencyBodyAcceleratorMagnitude Standard Deviation
- frequencyBodyAcceleratorMagnitude MeanFreq
- frequencyBodyBodyAcceleratorJerkMagnitude Mean
- frequencyBodyBodyAcceleratorJerkMagnitude Standard Deviation
- frequencyBodyBodyAcceleratorJerkMagnitude MeanFreq
- frequencyBodyBodyGyroscopeMagnitude Mean
- frequencyBodyBodyGyroscopeMagnitude Standard Deviation
- frequencyBodyBodyGyroscopeMagnitude MeanFreq
- frequencyBodyBodyGyroscopeJerkMagnitude Mean
- frequencyBodyBodyGyroscopeJerkMagnitude Standard Deviation
- frequencyBodyBodyGyroscopeJerkMagnitude MeanFreq


## Activity Labels
- 1 Walking: walking during the measurement
- 2 Walking_Up: walking up stairs during the measurement
- 3 Walking_Down: walking down stairs during the measurement
- 4 Sitting: sitting during the measurement
- 5 Standing: standing still during the measurement
- 6 Laying: laying down during the measurement


## What the code in 'run_analysis.R' will do (in order) when the script is run:
- Load dplyr 
- Load activity labels
- Load and select features that include mean or standard deviation
   Create list of feature names
   Transpose this list of feature names
   Make appropriate labels for the data set with descriptive variable names
   Coerce the proper dimensionality of the feature list
- Load training data
   Extract only the measurements on the mean and standard deviation for each measurement
   Appropriately label the data set with descriptive variable names
- Load testing data  
   Extract only the measurements on the mean and standard deviation for each measurement
   Appropriately label the data set with descriptive variable names
- Merge the training and the test sets to create one tidy data set: mydata
   Use descriptive activity names to name the activities in the data set
- Create a second, independent tidy data set with the average of each variable for each activity and each subject: mydata2
- Take averages for each activity
- Take averages for each subject
- Merge the two sets of averages
   Make Feature a labelled column rather than row names in accordance with tidy data theory
- View the first tidy data set: mydata
- View the second tidy data set: Finaldata


## Final Data Sets
- mydata: a dataset where all Features and Identifiers are variables and each row is a unique measurement for each subject and activity
- Finaldata: a dataset where each unique Identifier is a variable and each row is the set of averages of each variable for each activity 
and each subject
