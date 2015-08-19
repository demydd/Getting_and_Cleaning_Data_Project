The Manual how to run the script

1.to copy the file 'run_analysis.R'. The file is expected to install additional packages: 'dplyr' and 'reshape2'. The installation is launched automatically if these packages are not deployed at your PC.

2.Before running the code make sure to write the path variables correctly otherwise you will not read or write files properly.


Step-by-Step instructions to run the script

All steps are taken from the comments in the file 'run_analysis.R'
The packages and libraries are installed automatically if they have not been deployed (step 1 and 2).

to set paths variables: 

3 to set up the path to the directory that contains necessary files and folders "train", "test" (recommended to copy all files and folders to 'UCI HAR Dataset' folder

4 set up the path to the train directory

5 set up the path to the test directory

6 set up the path to the output directory(the place where the final set will be recorded)

7 set up working directory to read general info (root directory of UCI HAR Dataset)

8 Load: activity labels

9 Load: data column names

10 Load and process X_train & y_train data.

11 set up working directory to read train info

12 to read train info

13 to read train label info

14 to read train subject info

15 to add column names to train set

16 Extract only the measurements on the mean and standard deviation for each measurement.

17 Extract only the measurements on the mean and standard deviation for each measurement.

17.1 Load activity labels

18 Add names to activities

19 Bind all data into the targeted table of train data set

### to compile the test data we take all steps for train data set described in item 3-19

20 to merge all data (rows of train+test sets)

21 to define column name for the prfinal set

22 to make the prefinal set

23 to apply mean  to merged dataset using dcast function to compile the final set

24 to set the path for the output file (subject+activity+mean_per_factor)

25 to write a txt file with the final set
