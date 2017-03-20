# CATS-Basics
The basic repo for CATS assignment of B4TM on which students' work is based.

## Requirements for Git Repo

### Repo Name
Please check the repo name, if your repo name is not cats-2017-groupXX, please contact Cico for changing the name before you start your work here.

### Directory structure and folder names
You are required to follow the following directory structure and the folder names inside the repo to organize your code. The name of the folder or file with single star symbol should be the same with that in the structure below. The folder or file with double star symbols are the data or infomation provided by us, therefore changes are not recommended.

```
CATS-RepoName-of-YourGroup
│   README.md                 **
│   Summary.md                *
│   Estimate.txt              *
│   predication.txt           *
│
└───data                      **
│   │   Train_clinical.txt    **
│   │   Train_ca.txt          **
│   
└───model                     *
│   │   model.rds             *
│   │   model.pkl             *
│   │
└───code                      *
    │   file001.py
    │   file002.R
```

## Submission requirement

### Prediction
This file should be 'prediction.txt', the format has to be like this, which is delimited by tab:
```tt
"Sample"	"Subgroup"
"Array.1"	"Triple Neg"
"Array.61"	"HR+"
"Array.70"	"HER2+"
```

### Estimate
You need to hand in an estimate of how many of the 57 labels you have predicted correctly, based on your validation scheme. The answer should be a single number between 0 and 57, and be place in the file "Estimate.txt". The file looks like this:
```
57
```

### Scripts that build the best classifier
You should also hand in your R/Python scripts that build the classifier, predict the labels, and obtain the accuracy estimates. That is, the classifier that works best of all for you. All the codes should be placed under the directory of 'code'.

### Model file 
If your best classifier is created by R, please place it in model/model.rds; if Python, in model/model.pkl.

### Summary of results
Summary of your validation scheme results for all methods chosen also needs to be submitted. This part should be written into
'Summary.md'. You need to know something about markdown grammar.

### Submission deadline
All the stuff above should be submitted by **24 Apr 2017**, the last commit before the deadline will be counted in for grading.
