##Code Book
For the Human Activity Recognition Using Samsung Galaxy Smartphone tidy dataset TidyData.txt created by the run_analysis.R script.

###I. Raw data files


Data files that are used to create TidyData  is available from the unzipped raw dataset folder ‘UCI HAR Dataset’.

#####Training set

* train/X_train.txt: measurements for 561 variables

* train/y_train.txt: activity labels

* rain/subject_train.txt: subject identifier
 
#####Test set   

* test/X_test.txt: measurements for 561 variables
* test/y_test.txt: activity labels
* test/subject_t est.txt: subject identifier

#####Features/Variables

* features.txt: list of all features estimated from the measured signals

#####Activities

* activity_labels.txt: links activity labels to activity names

In addition, files README.txt and features_info.txt were used to infer infer information about the raw dataset measurements, files structure,  and variables.

###II. Notes on sumaries and omencature

Summary

* Variables [4:69]: are averaged, as mean values, for each subject and each activity.

Nomenclature

* body designates the volunteer person physical body.
* FFT designates the Fast Fourier Transform.
* X  (or Y,Z) direction designates the X axial direction.

###III. Variables units

•	 Variables [1:3]: categorical
•	 Variables [4:69]: normalized and bounded within [-1,1] 


###VI. Variables dictionnary

**1.Subject**
* Identifier assigned to the volunteer person who performed the experiment 
* Type:numeric
* Range: 1..30

**2.ActivityName**
* Daily-living activity performed by the person
* Type: character 
* Categories: WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING 

**3.ActivityNumber**
* Activity number 
* Type: number

**4.timeBodyAccelerometer.MEAN…X**
* Mean value of the body acceleration signal in the X direction 
* Type: numeric

**5.timeBodyAccelerometer.MEAN…Y**
* Mean value of the body acceleration signal in the Y direction
* Type: numeric

**6.timeBodyAccelerometer.MEAN…Z**
* Mean value of the body acceleration signal in the Z direction
* Type: numeric

**7.timeBodyAccelerometer.SD…X**
* Standard deviation of the body acceleration signal in the X direction
* Type: numeric

**8.timeBodyAccelerometer.SD…Y**
* Standard deviation of the body acceleration signal in the Y direction
* Type: numeric

**9.timeBodyAccelerometer.SD…Z**
* Standard deviation of the body acceleration signal in the Z direction
* Type: numeric

**10.timeGravityAccelerometer.MEAN…X**
* Mean value of the gravity force acceleration signal in the X direction
* Type: numeric

**11.timeGravityAccelerometer.MEAN…Y**
* Mean value of the gravity force acceleration signal in the Y direction
* Type: numeric

**12.timeGravityAccelerometer.MEAN…Z**
* Mean value of the gravity force acceleration signal in the Z direction
* Type: numeric

**13.timeGravityAccelerometer.SD…X**
* Standard deviation of the gravity force acceleration signal in the X direction
* Type: numeric

**14.timeGravityAccelerometer.SD…Y**
* Standard deviation of the gravity force acceleration signal in the Y direction
* Type: numeric


**15.timeGravityAccelerometer.SD…Z**
* Standard deviation of the gravity force acceleration signal in the Z direction
* Type: numeric

**16.timeBodyAccelerometerJerk.MEAN…X**
* Mean value of the body Jerk signal, as obtained from the acceleration, in the X direction
* Type: numeric

**17.timeBodyAccelerometerJerk.MEAN…Y**
* Mean value of the body Jerk signal, as obtained from the acceleration, in the Y direction
* Type: numeric

**18.timeBodyAccelerometerJerk.MEAN…Z**
* Mean value of the body Jerk signal, as obtained from the acceleration, in the Z direction
* Type: numeric

**19.timeBodyAccelerometerJerk.SD…X**
* Standard deviation of the body Jerk signal, as obtained from the acceleration, in the X direction
* Type: numeric

**20.timeBodyAccelerometerJerk.SD…Y**
* Standard deviation of the body Jerk signal, as obtained from the acceleration, in the Y direction   
* Type: numeric

**21.timeBodyAccelerometerJerk.SD…Z**
* Standard deviation of the body Jerk signal, as obtained from the acceleration, in the Z direction
* Type: numeric

**22.timeBodyGyroscope.MEAN…X**
* Mean value of the body angular velocity in the X direction
* Type: numeric

**23.timeBodyGyroscope.MEAN…Y**
* Mean value of the body angular velocity in the Y direction
* Type: numeric

**24.timeBodyGyroscope.MEAN…Z**
* Mean value of the body angular velocity in the Z direction
* Type: numeric

**25.timeBodyGyroscope.SD…X**
* Standard deviation of the body angular velocity in the X direction
* Type: numeric

**26.timeBodyGyroscope.SD…Y**
* Standard deviation of the body angular velocity in the Y direction
* Type: numeric

**27.timeBodyGyroscope.SD…Z**
* Standard deviation of the body angular velocity in the Z direction
* Type: numeric

**28.timeBodyGyroscopeJerk.MEAN…X**
* Mean value of the body Jerk signal, as obtained from the angular velocity, in the X direction
* Type: numeric

**29.timeBodyGyroscopeJerk.MEAN…Y**
* Mean value of the body Jerk signal, as obtained from the angular velocity, in the Y direction
*Type: numeric

**30.timeBodyGyroscopeJerk.MEAN…Z**
* Mean value of the body Jerk signal, as obtained from the angular velocity, in the Z direction
* Type: numeric

**31.timeBodyGyroscopeJerk.SD…X**
* Standard deviation of the body Jerk signal, as obtained from the angular velocity, in the X direction
* Type: numeric

**32.timeBodyGyroscopeJerk.SD…Y**
* Standard deviation of the body Jerk signal, as obtained from the angular velocity, in the Y direction
* Type: numeric

**33.timeBodyGyroscopeJerk.SD…Z**
* Standard deviation of the body Jerk signal, as obtained from the angular velocity, in the Z direction
* Type: numeric

**34.timeBodyAccelerometerMagnitude.MEAN..**
* Mean value of the magnitude of the body acceleration signal 
* Type: numeric

**35.timeBodyAccelerometerMagnitude.SD..**
* Standard deviation of the magnitude of the body acceleration signal 
* Type: numeric

**36.timeGravityAccelerometerMagnitude.MEAN..**
* Mean value of the magnitude of the gravity force acceleration signal 
* Type: numeric

**37.timeGravityAccelerometerMag.SD..**
* Standard deviation of the magnitude of the gravity force acceleration signal 
* Type: numeric

**38.timeBodyAccelerometerJerkMagnitude.MEAN..**
* Mean value of the magnitude of the body Jerk signal, as obtained from the acceleration 
* Type: numeric

**39.timeBodyAccelerometerJerkMagnitude.SD..**
* Standard deviation of the magnitude of the body Jerk signal, as obtained from the acceleration 
* Type: numeric

**40.timeBodyGyroscopeMagnitude.MEAN..**
* Mean value of the magnitude of the body angular velocity
* Type: numeric

**41.	timeBodyGyroscopeMag.SD..**
* Standard deviation of the magnitude of the body angular velocity
* Type: numeric

**42.	timeBodyGyroscopeJerkMagnitude.MEAN..**
* Mean value of the magnitude of the body Jerk signal, as obtained from the angular velocity 
* Type: numeric

**43.	timeBodyGyroscopeJerkMagnitude.SD..**
* Standard deviation of the magnitude of the body Jerk signal, as obtained from the angular velocity 
* Type: numeric

**44.	frequencyBodyAccelerometer.MEAN…X**
* Mean value of the FFT of the body acceleration signal in the X direction
* Type: numeric
 
**45.frequencyBodyAccelerometer.MEAN…Y**
* Mean value of the FFT of the body acceleration signal in the Y direction
* Type: numeric

**46.frequencyBodyAccelerometer.MEAN…Z**
* Mean value of the FFT of the body acceleration signal in the Z direction
* Type: numeric

**47.	frequencyBodyAccelerometer.SD…X**
* Standard deviation of the FFT of the body acceleration signal in the X direction
* Type: numeric

**48.	frequencyBodyAccelerometer.SD…Y**
* Standard deviation of the FFT of the body acceleration signal in the Y direction
* Type: numeric

**49.	frequencyBodyAccelerometer.SD…Z**
* Standard deviation of the FFT of the body acceleration signal in the Z direction
* Type: numeric

**50.frequencyBodyAccelerometerJerk.MEAN…X**
* Mean value of the FFT of the body Jerk signal, as obtained from the acceleration, in the X direction
*Type: numeric

**51.frequencyBodyAccelerometerJerk.MEAN…Y**
* Mean value of the FFT of the body Jerk signal, as obtained from the acceleration, in the Y direction
* Type: numeric

**52.frequencyBodyAccelerometerJerk.MEAN…Z**
* Mean value of the FFT of the body Jerk signal, as obtained from the acceleration, in the Z direction
* Type: numeric

**53.frequencyBodyAccelerometerJerk.SD…X**
* Standard deviation of the FFT of the body Jerk signal, as obtained from the acceleration, in the X direction
* Type: numeric

**54.	frequencyBodyAccelerometerJerk.SD…Y**
* Standard deviation of the FFT of the body Jerk signal, as obtained from the acceleration, in the Y direction
* Type: numeric

**55.frequencyBodyAccelerometerJerk.SD…Z**
* Standard deviation of the FFT of the body Jerk signal, as obtained from the acceleration, in the Z direction
* Type: numeric

**56.frequencyBodyGyroscope.MEAN…X**
* Mean value of the FFT of the body angular velocity in the X direction
* Type: numeric

**57.frequencyBodyGyroscope.MEAN…Y**
* Mean value of the FFT of the body angular velocity in the Y direction
* Type: numeric

**58.frequencyBodyGyroscope.MEAN…Z**
* Mean value of the FFT of the body angular velocity in the Z direction
* Type: numeric

**59.frequencyBodyGyroscope.SD…X**
* Standard deviation of the FFT of the body angular velocity in the X direction
* Type: numeric

**60.frequencyBodyGyroscope.SD…Y**
* Standard deviation of the FFT of the body angular velocity in the Y direction
* Type: numeric

**61.	frequencyBodyGyroscope.SD…Z**
* Standard deviation of the FFT of the body angular velocity in the Z direction
* Type: numeric

**62.	frequencyBodyAccelerometerMagnitude.MEAN..**
* Mean value of the magnitude of the FFT of the body acceleration signal 
* Type: numeric

**63.frequencyBodyAccelerometerMagnitude.SD..**
* Standard deviation of the magnitude of the FFT of the body acceleration signal 
* Type: numeric

**64.frequencyBodyAccelerometerJerkMagnitude.MEAN..**
* Mean value of the magnitude of the FFT of the body Jerk signal, as obtained from the acceleration 
* Type: numeric

**65.frequencyBodyAccelerometerJerkMagnitude.SD..**
* Standard deviation of the magnitude of the FFT of the body Jerk signal, as obtained from the acceleration 
* Type: numeric

**66.frequencyBodyGyroscopeMagnitude.MEAN..**
•	  Mean value of the magnitude of the FFT of the body angular velocity
•	  Type: numeric

**67.	frequencyBodyGyroscopeMagnitude.SD..**
* Standard deviation of the magnitude of the FFT of the body angular velocity
* Type: numeric

**68.frequencyBodyGyroscopeJerkMagnitude.MEAN..**
* Mean value of the magnitude of the FFT of the body Jerk signal, as obtained from the angular velocity 
* Type: numeric

**69.	frequencyBodyGyroscopeJerkMagnitude.SD..**
* Standard deviation of the magnitude of the FFT of the body Jerk signal, as obtained from the angular velocity 
* Type: numeric

