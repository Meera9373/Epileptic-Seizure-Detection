# Epileptic-Seizure-Detection
## Introduction

The aim of this study is to diagnose epileptic seizures by using different machine learning algorithms. 

For this purpose, the frequency components of the EEG are extracted by using the discrete wavelet transform (DWT) and parametric methods based on autoregressive (AR) model. 

Both these two feature extraction methods are applied to the input of machine learning classification algorithms such as Artificial Neural Networks (ANN), Naive Bayesian, k-Nearest Neighbor (k-NN), Support Vector Machines (SVM), Logistic Regression,Principal Component Analysis.

The results show that k-NN, ANN and SVM were the most efficient method according to test processing of both DWT and AR as feature extraction for recognition of epileptic seizures in EEG.

## Dataset

The original dataset from the reference consists of 5 different folders, each with 100 files, with each file representing a single subject/person. Each file is a recording of brain activity for 23.6 seconds.

The corresponding time-series is sampled into 4097 data points. Each data point is the value of the EEG recording at a different point in time. So we have a total of 500 individuals with 4097 data points for 23.5 seconds.

We divided and shuffled every 4097 data points into 23 chunks, each chunk contains 178 data points for 1 second, and each data point is the value of the EEG recording at a different point in time.

So now we have 23 x 500 = 11500 pieces of information(row), each information contains 178 data points for 1 second(column), the last column represents the label y {1,2,3,4,5}.

The response variable is y in column 179, the Explanatory variables X1, X2, ..., X178


## Result
![image](https://user-images.githubusercontent.com/60151306/184814844-48f4b308-b8f7-42e9-88df-54a971b2bbe5.png)
