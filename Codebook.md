Code Book
Description of the data and the transformations in order to clean data
Repository of the Data:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Description

Human Activity Recognition Using Smartphones Dataset
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz.
The experiments have been video-recorded to label the data manually.
The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

Contents

      train/X_train.txt: Training set.
      train/y_train.txt: Training labels
      test/X_test.txt: Test set.
      test/y_test.txt: Test labels
      README.txt
      features_info.txt:  Variables of the feature vector.
      features.txt
      activity_labels.txt: Relates labels to activity 
      train/subject_train.txt: Identifies each subject participating in the experiment (30)
      train/Inertial Signals/total_acc_x_train.txt: Signal measured by the smartphone accelerometer X axis in s units 'g'. 
      train/Inertial Signals/total_acc_x_train.txt: Signal measured by the smartphone accelerometer Y axis in s units 'g'. 
      train/Inertial Signals/total_acc_y_train.txt:  Signal measured by the smartphone accelerometer Z axis in s units 'g'. 
      train/Inertial Signals/body_acc_x_train.txt: Body acceleration signal X axis
      train/Inertial Signals/body_acc_y_train.txt: Body acceleration signal Y axis
      train/Inertial Signals/body_acc_z_train.txt: Body acceleration signal Z axis
      train/Inertial Signals/body_gyro_x_train.txt: Angular velocity vector measured by the gyroscope 
      
Data Transformations

1)Reading the dataset 

2)Merging the test and training datasets creating a unique data set. 

3)Selecting  the mean and standard deviation for each measurement. 

4)Using descriptive activity names to name the activities in the data set 

5)Labelling the data set with descriptive variable names. 

    • subject
    • activity_name
    •  tBodyAcceleration_Mean_X
    •  tBodyAcceleration_Mean_Y
    •  tBodyAcceleration_Mean_Z
    •  tgravityAcceleration_Mean_X
    •  tgravityAcceleration_Mean_Y
    •  tgravityAcceleration_Mean_Z
    •  tBodyAccelerationJerk_Mean_X
    •  tBodyAccelerationJerk_Mean_Y
    •  tBodyAccelerationJerk_Mean_Z
    •  tBodyGyroscope_Mean_X
    •  tBodyGyroscope_Mean_Y
    •  tBodyGyroscope_Mean_Z
    •  tBodyGyroscopeJerk_Mean_X
    •  tBodyGyroscopeJerk_Mean_Y
    •  tBodyGyroscopeJerk_Mean_Z
    •  tBodyAccelerationMagnitude_Mean
    •  tgravityAccelerationMagnitude_Mean
    •  tBodyAccelerationJerkMagnitude_Mean
    •  tBodyGyroscopeMagnitude_Mean
    •  tBodyGyroscopeJerkMagnitude_Mean
    •  FrequencyBodyAcceleration_Mean_X
    •  FrequencyBodyAcceleration_Mean_Y
    •  FrequencyBodyAcceleration_Mean_Z
    •  FrequencyBodyAcceleration_Meanfreq_X
    •  FrequencyBodyAcceleration_Meanfreq_Y
    •  FrequencyBodyAcceleration_Meanfreq_Z
    •  FrequencyBodyAccelerationJerk_Mean_X
    •  FrequencyBodyAccelerationJerk_Mean_Y
    •  FrequencyBodyAccelerationJerk_Mean_Z
    •  FrequencyBodyAccelerationJerk_Meanfreq_X
    •  FrequencyBodyAccelerationJerk_Meanfreq_Y
    •  FrequencyBodyAccelerationJerk_Meanfreq_Z
    •  FrequencyBodyGyroscope_Mean_X
    •  FrequencyBodyGyroscope_Mean_Y
    •  FrequencyBodyGyroscope_Mean_Z
    •  FrequencyBodyGyroscope_Meanfreq_X
    •  FrequencyBodyGyroscope_Meanfreq_Y
    •  FrequencyBodyGyroscope_Meanfreq_Z
    •  FrequencyBodyAccelerationMagnitude_Mean
    •  FrequencyBodyAccelerationMagnitude_Meanfreq
    •  FrequencyBodybodyAccelerationJerkMagnitude_Mean
    •  FrequencyBodybodyAccelerationJerkMagnitude_Meanfreq
    •  FrequencyBodybodyGyroscopeMagnitude_Mean
    •  FrequencyBodybodyGyroscopeMagnitude_Meanfreq
    •  FrequencyBodybodyGyroscopeJerkMagnitude_Mean
    •  FrequencyBodybodyGyroscopeJerkMagnitude_Meanfreq
    •  tBodyAcceleration_StandardDeviation_X
    •  tBodyAcceleration_StandardDeviation_Y
    •  tBodyAcceleration_StandardDeviation_Z
    •  tgravityAcceleration_StandardDeviation_X
    •  tgravityAcceleration_StandardDeviation_Y
    •  tgravityAcceleration_StandardDeviation_Z
    •  tBodyAccelerationJerk_StandardDeviation_X
    •  tBodyAccelerationJerk_StandardDeviation_Y
    •  tBodyAccelerationJerk_StandardDeviation_Z
    •  tBodyGyroscope_StandardDeviation_X
    •  tBodyGyroscope_StandardDeviation_Y
    •  tBodyGyroscope_StandardDeviation_Z
    •  tBodyGyroscopeJerk_StandardDeviation_X
    •  tBodyGyroscopeJerk_StandardDeviation_Y
    •  tBodyGyroscopeJerk_StandardDeviation_Z
    •  tBodyAccelerationMagnitude_StandardDeviation
    •  tgravityAccelerationMagnitude_StandardDeviation
    •  tBodyAccelerationJerkMagnitude_StandardDeviation
    •  tBodyGyroscopeMagnitude_StandardDeviation
    •  tBodyGyroscopeJerkMagnitude_StandardDeviation
    •  FrequencyBodyAcceleration_StandardDeviation_X
    •  FrequencyBodyAcceleration_StandardDeviation_Y
    •  FrequencyBodyAcceleration_StandardDeviation_Z
    •  FrequencyBodyAccelerationJerk_StandardDeviation_X
    •  FrequencyBodyAccelerationJerk_StandardDeviation_Y
    •  FrequencyBodyAccelerationJerk_StandardDeviation_Z
    •  FrequencyBodyGyroscope_StandardDeviation_X
    •  FrequencyBodyGyroscope_StandardDeviation_Y
    •  FrequencyBodyGyroscope_StandardDeviation_Z
    •  FrequencyBodyAccelerationMagnitude_StandardDeviation
    •  FrequencyBodybodyAccelerationJerkMagnitude_StandardDeviation
    •  FrequencyBodybodyGyroscopeMagnitude_StandardDeviation
    •  FrequencyBodybodyGyroscopeJerkMagnitude_StandardDeviation

6)Generating  a second, independent tidy data set with the average of each variable for each activity and each subject.
