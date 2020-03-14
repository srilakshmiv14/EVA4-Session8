# EVA4-Session8

1.	Importing all the packages.
2.	Modules are stored in a library which is available in Session 8 repository folder named Library.
3.	Modules are    1. Loading Data
      2. Transforming the data 
      3. Building the Basic Model
      4. ResNet-18 Model
      5. Training and testing the model.

             Modules Description:      
(i)	Loading CIFAR 10 Datasets.

(ii)	 Transformations done:

Augmentations:
1.	RandomRotation()
2.	RandomHorizontalFlip()
3.	RandomErasing()

(iii)	Loading and running Train dataset and Test dataset:
1.	#Implementing L1 regularization
 if self. L1lambda > 0:
     reg_loss = 0.
  		    for param in self. model. parameters ():
 		        reg_loss += torch. sum (param. abs ())
    		        loss += self. L1lambda * reg_loss
               
2.	We have used SGD Optimizer with learning rate 0.01% and Momentum 0.9 and included LR Scheduler as well with step size 5 and gamma 0.5.

3.	Model parameters are 11,173,962 


4.	Ran the model with 20 epochs 
Train set: Average loss: 0.0012, Accuracy: 94.57%; 
Test set: Average loss: 0.2720, Accuracy: 91.66%

Final Accuracy of the model is 91.66%




