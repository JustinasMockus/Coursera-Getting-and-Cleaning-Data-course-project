# Introduction

The script `run_analysis.R`
- downloads the data from
  [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/index.html).
- merges the training and test sets to create one data set.
- appropriately labels the columns with descriptive names.
- extracts only the measurements (features) on the mean and standard deviation
  for each measurement.
- replaces `Activity` values in the dataset with descriptive activity names.
- creates a second tidy dataset with an average of each variable.
  for each activity and each subject.Then tidy data.
  set is also exported as txt file.
  
# Variables

* `TrainData`, `TrainActivity`, `TestData`, `TestActivity`, `TrainSubjects` and `TestSubjects` contain the data from the downloaded files.
* `TrainDataSet`, `TestDataSet` are merged to `CombinedDataSet` for further analysis.
* `FeatureNames` contains the correct names for the `TrainData` dataset.
* `MeanStdColumns` variable is used to extract columns which contain mean and standart deviation.
* `MeanStdDataSet` are created from variables `SubjectID`,`ActivityID`, `MeanStdColumns`.
* `ActivityLabels` contains activity labels and is used to add labels to `MeanStdDataSet` data frame.
* `TidyMelt` contains data after melt function.
* `TidyData` is a final data set of tidy data.

# Transformation details

There are 5 parts:

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
