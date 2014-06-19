<pre>
DATA DICTIONARY
FOR
ACCELEROMETER DATA 
FROM SAMSUNG GALAXY S SMARTPHONE

Source datafiles:
	- subject_test.txt
	- X_test.txt
	- y_test.txt
	- subject_train.txt
	- X_train.txt
	- y_train.txt

subject_id
	Description:  subject identifier
	Datatype:  numeric
	Range:  1 .. n
	
activity_type
	Description:  activity description
	Datatype:  alphanumeric
	Range:  WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING
	Note:  The original datafile contained numeric values from 1 to 6 representing the above
	       activities:  
			1 WALKING
			2 WALKING_UPSTAIRS
			3 WALKING_DOWNSTAIRS
			4 SITTING
			5 STANDING
			6 LAYING		   
		   The actual activity name is stored in this dataset.  See activity_labels.txt
	
tBodyAcc-mean()-X
tBodyAcc-mean()-Y
tBodyAcc-mean()-Z
	Description:  The calculated mean of accelerometer 3-axial raw signals of body acceleration 
		along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	
tBodyAcc-std()-X
tBodyAcc-std()-Y
tBodyAcc-std()-Z
	Description:  The calculated standard deviation of accelerometer 3-axial raw signals of body 
		acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tGravityAcc-mean()-X
tGravityAcc-mean()-Y
tGravityAcc-mean()-Z
	Description:  The calculated mean of accelerometer 3-axial raw signals of gravitational 
		acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tGravityAcc-std()-X
tGravityAcc-std()-Y
tGravityAcc-std()-Z
	Description:  The calculated standard deviation of accelerometer 3-axial raw signals of 
		gravitational acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyAccJerk-mean()-X
tBodyAccJerk-mean()-Y
tBodyAccJerk-mean()-Z
	Description:  The calculated mean of accelerometer 3-axial raw signals of body linear 
		acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyAccJerk-std()-X
tBodyAccJerk-std()-Y
tBodyAccJerk-std()-Z
	Description:  The calculated standard deviation of accelerometer 3-axial raw signals of body 
		linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyro-mean()-X
tBodyGyro-mean()-Y
tBodyGyro-mean()-Z
	Description:  The calculated mean of gyroscope 3-axial raw signals of body acceleration 
		along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	  
tBodyGyro-std()-X
tBodyGyro-std()-Y
tBodyGyro-std()-Z
	Description:  The calculated standard deviation of gyroscope 3-axial raw signals of body 
		acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyroJerk-mean()-X
tBodyGyroJerk-mean()-Y
tBodyGyroJerk-mean()-Z
	Description:  The calculated mean of accelerometer 3-axial raw signals of body 
		linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyroJerk-std()-X
tBodyGyroJerk-std()-Y
tBodyGyroJerk-std()-Z
	Description:  The calculated standard deviation of accelerometer 3-axial raw signals of body 
		linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	  
tBodyAccMag-mean()
	Description:  The calculated Euclidean norm mean of accelerometer 3-axial raw signals of body 
		acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyAccMag-std()
	Description:  The calculated Euclidean norm standard deviation of accelerometer 3-axial raw 
		signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tGravityAccMag-mean()
	Description:  The calculated Euclidean norm mean of accelerometer 3-axial raw signals of 
		gravitational acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tGravityAccMag-std()
	Description:  The calculated Euclidean norm standard deviation of accelerometer 3-axial raw 
		signals of gravitational acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyAccJerkMag-mean()
	Description:  The calculated Euclidean norm mean of accelerometer 3-axial raw signals of 
		body linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyAccJerkMag-std()
	Description:  The calculated Euclidean norm standard deviation of accelerometer 3-axial raw 
		signals of body linear acceleration and angular velocity derived in time along the X, Y, 
		or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyroMag-mean()
	Description:  The calculated Euclidean norm mean of accelerometer 3-axial raw signals of body 
		linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyroMag-std()
	Description:  The calculated Euclidean standard deviation of accelerometer 3-axial raw signals 
		of body linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

tBodyGyroJerkMag-mean()
	Description:  The calculated Euclidean norm mean of accelerometer 3-axial raw signals of body 
		linear acceleration and angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	  
tBodyGyroJerkMag-std()
	Description:  The calculated Euclidean norm standard deviation of accelerometer 3-axial raw 
		signals of body linear acceleration and angular velocity derived in time along the X, Y, 
		or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyAcc-mean()-X
fBodyAcc-mean()-Y
fBodyAcc-mean()-Z
	Description:  The calculated mean with an applied FFT (Fast Fourier Transform) of accelerometer 
		3-axial raw signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	  
fBodyAcc-std()-X
fBodyAcc-std()-Y
fBodyAcc-std()-Z
	Description:  The calculated standard deviation with an applied FFT (Fast Fourier Transform) 
		of accelerometer 3-axial raw signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyAccJerk-mean()-X
fBodyAccJerk-mean()-Y
fBodyAccJerk-mean()-Z
	Description:  The calculated mean with an applied FFT (Fast Fourier Transform) of accelerometer 
		3-axial raw signals of body linear acceleration and angular velocity derived in time along 
		the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyAccJerk-std()-X
fBodyAccJerk-std()-Y
fBodyAccJerk-std()-Z
	Description:  The calculated standard deviation with an applied FFT (Fast Fourier Transform)
		of accelerometer 3-axial raw signals of body linear acceleration and angular velocity 
		derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyGyro-mean()-X
fBodyGyro-mean()-Y
fBodyGyro-mean()-Z
	Description:  The calculated mean with an applied FFT (Fast Fourier Transform) of gyroscope 
		3-axial raw signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyGyro-std()-X
fBodyGyro-std()-Y
fBodyGyro-std()-Z
	Description:  The calculated standard deviation with an applied FFT (Fast Fourier Transform) 
		of gyroscope 3-axial raw signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyAccMag-mean()
	Description:  The calculated Euclidean norm mean with an applied FFT (Fast Fourier Transform) 
		of accelerometer 3-axial raw signals of body acceleration along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyAccMag-std()
	Description:  The calculated Euclidean norm standard deviation with an applied FFT (Fast 
		Fourier Transform)of accelerometer 3-axial raw signals of body acceleration along the 
		X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyBodyAccJerkMag-mean()
	Description:  The calculated Euclidean norm mean with an applied FFT (Fast Fourier Transform) 
		of accelerometer 3-axial raw signals of body linear acceleration and angular velocity 
		derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt
	  
fBodyBodyAccJerkMag-std()
	Description:  The calculated Euclidean norm standard deviation with an applied FFT (Fast 
		Fourier Transform) of accelerometer 3-axial raw signals of body linear acceleration and 
		angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyBodyGyroMag-mean()
	Description:  The calculated Euclidean norm mean with an applied FFT (Fast Fourier Transform) 
		of accelerometer 3-axial raw signals of body linear acceleration and angular velocity 
		derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyBodyGyroMag-std()
	Description:  The calculated Euclidean norm standard deviation with an applied FFT (Fast 
		Fourier Transform) of accelerometer 3-axial raw signals of body linear acceleration and 
		angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyBodyGyroJerkMag-mean()
	Description:  The calculated Euclidean norm mean with an applied FFT (Fast Fourier Transform) 
		of accelerometer 3-axial raw signals of body linear acceleration and angular velocity 
		derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

fBodyBodyGyroJerkMag-std()
	Description:  The calculated Euclidean norm standard deviation with an applied FFT (Fast 
		Fourier Transform) of accelerometer 3-axial raw signals of body linear acceleration and 
		angular velocity derived in time along the X, Y, or Z axis.
	Datatype:  numeric
	Range:  -1 .. 1
	Note:  
	  Source files:  X_test.txt, Y_test.txt, X_train.txt, Y_train.txt

	  
## END OF FILE -------------------------------------------------------------------------------------	  
</pre>