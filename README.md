# AWS Linear Learner (Salary Prediction)
Employee Salary Predictions Using AWS Sagemaker Linear Learner
Project Overview: The objective is to predict the employee salary based in the number of exprience.


**Preprocessing**:
1. Data should be suffled before training.
2. Data has to be normalized. (feature scaling is offered by AWS)

**Training**:
1. Linear Learner uses stochastic gradient descent
2. Optimizer: Adam, AdaGrad, SGD
3. Hyperparameters: Learning rate, epochs, batch size, predictor_type, etc.,
4. Regularization to avoid overfitting
5. Multiple models could be optimized in parallel 

**Validation**:
Evaluate the model based on MSE, MAE, cross entropy loss, absolute error

**Input/Output Data**:
Linear Learner supports 
      (Input Data),
      1. RecordIO-wrapped protobuf 
      2. Text/SCv (I column to be the target label)
      3. File or pipe mode
      (Output Data),
      1. Json
      2. x-recordio-protobuf
      3. text/csv
      
**EC2 Instances: Single CPU is used for this project**

### Steps in AWS Sagemaker
+ Step 1 - > 
     a. Instantiate a Notebook Instance
        (or)
     b. Instantiate AWS SM Studio
+ Step 2 - > Import Key libraries and dataset
+ Step 3 - > Perform Exploratory Data Analysis
+ Step 4 - > Create training & testing dataset
+ Step 5 - > Train a Linear Regeression Model in Sklearn
+ Step 6 - > Evaluate trained model performance
+ Step 7 - > Train a linear learner model in SageMaker
+ Step 8 - > Deploy model & invoke endpoint in SageMaker


