# Human-Activity-recognition-study

This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying.
This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.


How data was recorded
By using the sensors(Gyroscope and accelerometer) in a smartphone, they have captured '3axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations.
prefix 't' in those metrics denotes time.
suffix 'XYZ' represents 3-axial signals in X , Y, and Z directions

Quick overview of the dataset :
Accelerometer and Gyroscope readings are taken from 30 volunteers(referred as

subjects) while performing the following 6 Activities.

1. Walking 
2. WalkingUpstairs 
3. WalkingDownstairs 
4. Standing 
5. Sitting 
6. Lying.
7. 
Readings are divided into a window of 2.56 seconds with 50% overlapping. Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y and z components each. 

Gyroscope readings are the measure of angular velocities which has x,y and z components. 

Jerk signals are calculated for BodyAcceleration readings.

Fourier Transforms are made on the above time readings to obtain frequency readings.

Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.

We get a feature vector of 561 features and these features are given in the dataset. 

Each window of readings is a datapoint of 561 features.

Problem Framework 

30 subjects(volunteers) data is randomly split to 70%(21) test and 30%(7) train data. 

Each datapoint corresponds one of the 6 Activities.
