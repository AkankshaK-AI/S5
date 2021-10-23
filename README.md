# S5Assignment
**Step 1:**

Target- to reach 99.4% accuracy within 10 epochs

Get the set-up right
Set Transforms
Set Data Loader
Set Basic Working Code
Set Basic Training & Test Loop

Results:

Parameters: 6.3M
Best Training Accuracy: 99.86
Best Test Accuracy: 99.27

Analysis: 
Extremely heavy model with large number of parameters
Overfitting


**Step 2:**

Target: 
Get the basic skeleton right. 
Reduce the parameters to reach the target of 20k parameters within 15 epochs
Reach the model accuracy at 99.4%
We want the overfitting number to be very small

Results:
Parameters: 194,884
Best Training Accuracy: 99.29
Best Test Accuracy: 98.89

Analysis: 
Model is still large with lesser than target accuracy. 
We see Overfitting. 


**Step 3**

Target: 
Make the model lighter
Reduce the parameters to reach the target of 10k parameters within 15 epochs
Reach the model accuracy at 99.4%
We want the overfitting number to be very small

Results:
Parameters: 10,790
Best Training Accuracy: 98.93(15th epoch)
Best Test Accuracy: 98.92(14th epoch)

Analysis: 
Model is small with less than targeted accuracy
We see overfitting in the 15th epoch. In the 10th, 11th, 13th and 14th epoch, we have witnessed underfitting of of the model
