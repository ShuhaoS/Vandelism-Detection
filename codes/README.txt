Instructions for running the code:
The run.sh files are inside tensorflow/sklearn


For tensor flow:
Depedencies:

For data_to_csv.py:
"codecs": was needed for dealing with unicode characters,
"lxml": was used for parsing the xml into trees
"tqdm": was used for progress bars in the terminal window

For csv_to_tensor.py:
Python version 3.5
"pandas" was used for metrics about the data

Running the code:
1. Aquire the training, validation, and test data from http://www.wsdm-cup-2017.org/vandalism-detection.html

2. Extract it into their respective directories, named: data/tensorflow/Train, data/tensorflow/Validation, and data/tensorflow/Test

3. Run data_to_csv.py. This will generate the csv files needed for training and testing the models
> py data_to_csv.py

4. Run csv_to_tensor.py
> py -3.5 csv_to_tensor.py

OR Just run the shell script that executes 3. and 4. 





For sklearn:
Dependencies:
Python 3
For sckit_data_to_csv.py:
"codecs": was needed for dealing with unicode characters,
"lxml": was used for parsing the xml into trees
"tqdm": was used for progress bars in the terminal window
For sckit_train_LSVC.py/ sckit_train_SVC.py:
"pandas" was used for metrics about the data
"scipy"/"sklearn" was used for classification

Running the code:
1. Aquire the training, validation, and test data from http://www.wsdm-cup-2017.org/vandalism-detection.html

2. Extract it into their respective directories, named: data/sklearn/Train, data/sklearn/Validation

3. Run sckit_data_to_csv.py. This will generate the csv files needed for training and testing the models
> py sckit_data_to_csv.py

4. Run sckit_train_LSVC.py for LinearSVC classifier or sckit_train_SVC.py for SVC with linear kernel
> py sckit_train_LSVC.py/sckit_train_SVC.py

