# S5Assignment
**Step 1:** Basic Skeleton

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


**Step 2:** Adding the Convolution blocks

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


**Step 3** Reducing the no. of parameters

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


**Step 4** Adding Batch Normalization

Target: 
Increase the no. of parameters slightly
Reach the model accuracy at 99.4%
We want the overfitting number to be very small

Results:
Parameters: 10,970
Best Training Accuracy: 99.75
Best Test Accuracy: 99.23

Analysis: 
Accuracy has improved a lot with batch normalization. We could reach the target of 99.4 on training within epoch 7
We see overfitting in the model.


**Step 5** Adding Regularization- Dropout

Target: 
Decrease the gap between train and test
Reach the model accuracy at 99.4%


Results:
Parameters: 10,970. Dropout doesnt add parameters hence same as before.
Best Training Accuracy: 99.24 (epoch 15th)
Best Test Accuracy: 99.13 (epoch 11th)

Analysis: 
Lower than target accuracy. Big sized kernel is used. Slight overfitting still exists


**Step 6** Adding Average pooling

Target: 
Get rid of the big kernel(7*7) because of large weights and replace with GAP layer.
Reach the model accuracy at 99.4%


Results:
Parameters: 6,070. Reduced drastically.
Best Training Accuracy: 98.59 (epoch 15th)
Best Test Accuracy: 98.07 (epoch 13th)

Analysis: 
Model's accuracy is impacted due to reduced number of parameters hence we need to add back few parameters.


**Step 7** Increasing the capacity- no. of parameters

Target: 
Increase the no. of parameters to improve model accuracy to reach 99.4%


Results:
Parameters: 11,994.
Best Training Accuracy: 99.24 (epoch 15th)
Best Test Accuracy: 99.08 (epoch 11th)

Analysis: 
Accuracy has improved but still less than target.
Still overfitting
We need to add dropout to every layer and not just a specific layer as we dont know which layer is causing over-fitting.


**Step 8** Correcting Max Pooling location, adding dropout to every layer, decreasing dropout value to 0.1

Target: 
To make corrections in the model to reduce overfitting.
To add dropout to every layer


Results:
Parameters: 13,808
Best Training Accuracy: 99.13 (epoch 13th)
Best Test Accuracy: 99.40 (epoch 13th) & 99.41(epoch 15th)

Analysis: 
We hit out test target twice. 
Model is now underfitting

