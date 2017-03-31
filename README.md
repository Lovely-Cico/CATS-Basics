# About the assignment

## Requirements for the team Git repo

### Repo name
Please check the repo name, if your repo name is not cats-2017-groupXX, please contact Cico for changing the name before you start your work here.

### Directory structure and folder names
You are required to follow the following directory structure and the folder names inside the repo to organize your code. The name of the folder or file with single star symbol should be the same with that in the structure below. The folder or file with double star symbols are the data or infomation provided by us, therefore changes are not recommended.
   
```
CATS-RepoName-of-YourGroup
│   README.md                 **
│   estimate.txt              *
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
└───codes                      *
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

## Programming languages and software
To play with machine learning, you need some tools that have already framed the methods,so that you can use them without extra efforts, if reading documentation is not deemed to be the 'extra effort'. In this assignment, we recommend you to use R or Python.

### R
If you feel comfortable with R, you can try the R package 'caret', which has been installed in the computer classroom. If you are not familiar with R, you can start it by reading the tutorial we provided.

### Python
If you go for Python, [scikit-learn](http://scikit-learn.org/stable/) is recommended. Basic knowledge of [NumPy](http://www.numpy.org/) will be helpful; advanced users can try [Pandas](http://scikit-learn.org/stable/tutorial/basic/tutorial.html) and [sklearn-pandas](https://github.com/paulgb/sklearn-pandas) to make more sensible data transformation. We recommend using Python 3.5+ instead of Python2 (if not necessary) for you assignment.

## Why to save your best model into files
In practice, training is usually computationally expensive and therefore time-comsuming. If you get it a good estimator (or a classifier in the assignment), it is best to save it into file, so that you can reuse it in the future just by reading the file into the variable obviating the need to retrain the model. 
