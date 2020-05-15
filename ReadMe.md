In this project I have applied a feed forward Neural Network to FARS dataset. This is following the implemenatation of the "Abdelwahab, H. T. and Abdel-Aty, M. A. (2001) ‘Development of Artificial Neural Network Models to Predict Driver Injury Severity in Traffic Accidents at Signalized Intersections’. 
The main purpose of this project is to examine the relationship between driver injury severity, driver, vehicle and roadway condition. For this purpose multi-layered feed forward neural network is used.Driver severity injury was divided into four main discrete categories (discussed below in detail) making this model a pattern recognition task.In the below sections we will discuss in detail the dataset used, pre-processing performed, Neural network developed, results obtained and what we can conclude from those results.

DATASET 

The dataset used was Fatal Analysis Reporting System (FARS) [3]. The data is collected from accidents across the United States from 1975 to 2018 (according to the last update). It has approximately 10 to 100 thousand observations and NHTSA has these datasets stored in their website which is available and accessible to the public. For the purpose of this paper, data of only 2018 was used, which consisted of around 70,000 records. The dataset consisted of large number of attributes, out of which only 8 attributes was selected which were thought to contribute the most for this task. Attributes and their brief description is as followed:
• MAN_COLL: Manner of Collision.
• AGE: Age of the Driver
• SEX: Sex of the driver
• DRUGS: Drugs were involved for this person
• DRUNK_DR: if the driver was drunk or not
• TYP_INT: Type of intersection
• LGT_COND: Light condition at the time of the accident
• CAR_AGE: Age of the car

Pre-Processing
The Data that was taken from the FARS couldn’t be taken as it is for the ANN. Following are the pre-processing that was done before passing it to the ANN.
Some of the attributes had values that were similar and didn’t contribute much to the training of the model, thus they were removed. For the Manner of collision originally had 11 classes but it was reduced to 5 classes- unknown, side sweep, rear and front. Fig.1. Shows the distribution of data before and fig.2 shows after.


![alt text](https://github.com/happysisodia/NN-Injury-Severity/tree/master/Images/pre_1.JPG?raw=true)




