<pre>
Filename:  README.md
----------------------------------------------------------------------------------------------------
Directory contents:
  - CodeBook.md
    - Data transformation/cleaning information
  - README.md
    - this file
  - run_analysis.R
    - R program code
  - run_analysis.out
    - Program output file.


Preliminary setup:
1.  Download datafile (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
    and save in a directory named "data".
2.  Extract the ZIP archive file in the current directory, data.  A directory, UCI HAR Dataset, will
    be created.  When this step is complete, the directory structure will be as follows:

</pre>
	
	./                                <-- location of R file, run_analysis.R
	./data                            <-- download location of ZIP file
	./data/UCI HAR Dataset            <-- created when ZIP archive expanded
	                      /activity_labels.txt
						  /features.txt
						  /features_info.txt
						  /README.txt
	./data/UCI HAR Dataset/test
	                           /subject_test.txt
							   /X_test.txt
							   /y_test.txt
	./data/UCI HAR Dataset/test/Inertial Signals
												/body_acc_x_test.txt
												/body_acc_y_test.txt
												/body_acc_z_test.txt
												/body_gyro_x_test.txt
												/body_gyro_x_test.txt
												/body_gyro_y_test.txt
												/body_gyro_z_test.txt
												/total_acc_x_test.txt
												/total_acc_y_test.txt
												/total_acc_z_test.txt
	./data/UCI HAR Dataset/train
	                           /subject_train.txt
							   /X_train.txt
							   /y_train.txt
	./data/UCI HAR Dataset/train/Inertial Signals
												/body_acc_x_train.txt
												/body_acc_y_train.txt
												/body_acc_z_train.txt
												/body_gyro_x_train.txt
												/body_gyro_x_train.txt
												/body_gyro_y_train.txt
												/body_gyro_z_train.txt
												/total_acc_x_train.txt
												/total_acc_y_train.txt
												/total_acc_z_train.txt

<pre>												
Program analysis
================
The program, run_analysis.R, performs the following operations (details can be found in the file,
run_analysis.out):

NOTE:  The following data files:  subject_test.txt, X_test.txt, y_test.txt, subject_train.txt,
		X_train.txt, and y_train.txt are referenced in the above program.  These files must
		be located in the same directory as the run_analysis.R file.
		
							   
1.  Merge the training and the test sets to create one data set.
  a.  The data was first divided into a "test" and a "train" dataset.
  b.  From there, there were three separate files,
	  - subject file which specifies the subject identifier
	  - X file which defines various measurement data.  Column information for each of the 561
		fields can be found in the file, features.txt.
	  - Y file which defines the activity id.  Descriptive text for each id can be found in
		the file, activity_labels.txt.
  c.  Read test data
	  - read subject data, subject_test.txt
	  - read X data, X_test.txt
	  - read Y data, Y_test.txt
  d.  Combine the three test files into a single dataset.
      - Since each file represents a column of data and each dataset has the same number of rows, 
	    combine them column wise using R's cbind() command.
  e.  Read train data
	  - read subject data, subject_train.txt
	  - read X data, X_train.txt
	  - read Y data, Y_train.txt
  d.  Combine the three train files into a single dataset.
      - Since each file represents a column of data and each dataset has the same number of rows, 
	    combine them column wise using R's cbind() command.
  e.  Combine the test and train datasets into a single dataset.
      - There is no need to differentiate between the test or train measurements.
	  - Use R's rbind() command to combine the two datasets into one large dataset.
	
2.  Extract only the measurements on the mean and standard deviation for each measurement. 
  a.  Identify those columns in the features.txt file that are related to mean and standard
		deviation.  In this case, perform a search for "mean()" and "std()".  Although there are 
		other columns with "mean" in them the corresponding measurement may not have a standard
		deviation.

3.  Use descriptive activity names to name the activities in the data set.  Appropriately label the 
    data set with descriptive variable names. 
  a.  Utilize the column names from the features.txt file to label the measurement data.
  b.  Utilize the activity descriptions from the activity_labels.txt file to identify the 
	    activities.
  c.  Add a new column to the dataset describing the activity.	
	
4.  Create a second, independent tidy data set with the average of each variable for each 
    activity and each subject. 
  a.  Group the data by subject and activity and for each measurement data point, calculate the
	    average.
  b.  Write this "tidy" data to a file.  Why is the data tidy?
	  - Each variable forms a columns.
		  - Each mean and standard deviation observation is in its own column.
		  - Each observation forms a row.
		  - The data is ordered by subject_id and activity type.
	  - Each table/file stores data about one kind of observation.
		  - Measurement data obtained from Samsung smartphone. 

		  
Lessons Learned:
1.  The above program was executed on a Windows 7 64-bit Xeon 3.30 GHz machine with
    28 GB of RAM; so memeory was not an issue.
2.  With much of the information being loaded into memory and not removed, this program will
    probably not run on machines with under 8 GB of RAM.
3.  Freeing up objects with the rm() command may reduce the memory requirements.


TODO:
1.  Improve performance.
2.  Reduce memory requirements.

</pre>
