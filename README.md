###Getting and Cleansing data collected from the accelerometers of the Samsung Galaxy S smartphone
####Author: Pinaki Patra (PP) – Date: Tuesday, May 10, 2016

#####Project summary:
Collect and process the Human Activity Recognition Using Samsung Galaxy S Smartphone to create the tidy dataset TidyData.txt. 
The raw data is available at the website  https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip .
Data processing is achieved by means of the run_analysis.R script while CoodBook.md serves as a detailed Code Book for TidyData.txt.

#####Table of contents:

1.README.md (this file).

2.run_analysis.R

3.CodeBook.md

#####Data description

######The raw dataset

Details about The Human Activity Recognition Using Smartphones Dataset experiments are available using this link as well as from the measurements associated ‘README.txt’ file. The database was collected in experiments using recordings of 30 volunteers (Subject), aged [19-48], performing daily-living activities  while carrying a waist-mounted Samsung Galaxy S II smartphone. 
The smartphone was equipped with two sensors: an accelerometer and a gyroscope that recorded the 3-axial linear acceleration and 3-axial angular velocity signals of the subject respectively.The experiments were video-recorded to label the data manually. 
The measurements were randomly partitioned into two sub-sets: Training (70%) and Test (30%).

######The tidy dataset

The raw data files used to create the tidy set TidyData.txt is submitted as part of this assignment. 
Data processing performed by run_analysis.R includes:

1.Downloading the files and unzipping it.

2.Loading the required packages like dplyr,data.table and tidyR

3.Read the corresponding files in two data sets and merge them

4.Subsetting to retain only a set of variables

5.Change the existing variable names and provide meaningful descriptive names

6.And finally aggregating these variables as averages per Subject and per Activity

 
In particular,TidyData.txt has:

1.Each variable stored in one column.

2.Each row provides a different observation of that variable.

######run_analysis.R 

script that processes the raw data to create the TidyData.txt tidy dataset. 
The latter dataset is saved to the TidyData.txt file and can be loaded with read.table() specifying the parameter header=TRUE. 

In summary, the script:

Read the Data

1.Downloads the raw dataset archive (.zip) file to the local working directory.

2.Reads the data files of interest using read.table() function.

Processes the raw data

1.Load the required R packages 

2.Combine the corresponding activity , ssubject and data files from two data sets  using rbind

3.Rename the column of combined activity and combined subject dataframe

4.Rename the name of columns of datatable according to the names provided in feautures.txt file

5.Merge the columns final activity and subject using cbind

6.Merge the columns of datatable dataframe with the datframe obtained in step 5

7.Subsets each measurements set (Training,Test) to retain only the ‘mean()’ and ‘std()’ variables or features estimated from the signals.

8.Enter the name of activity into the dataframe obtained in step 8 by joining with activitylabels as provided in acivitylable.txt file

9.Change the variable names and provide meaningful variable names

10.Create  a final daaset, using average( arithmetic mean) by each subject/person and actibity using aggregate function

11.Sort the data by subject and activity and then write to the file TidyData.txt


######CodeBook.md

Code Book for the tidy dataset TidyData.txt. It summarizes the raw data files employed by run_analysis.R as well as dataTable’s variables units and dictionary


