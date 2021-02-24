# Electric_Motor_Temperature
Predicting Motor temperature using Deep Learning (LSTM) and ML models (Random Forest, SVM and Linear Regressor)   
  
Steps to run the code :  
1. In order to make the data compatible to be run with the Machine Learning models, we need to ensure the data is in the correct form. First download the data from [Kaggle](https://www.kaggle.com/wkirgsn/electric-motor-temperature).   
2. After downloading the data, place the code files and data, run the [data pre-processing code](https://github.com/mjaju/Electric_Motor_Temperature/blob/main/Code%20and%20Data%20Files/Pre-Processing%20Raw%20data.ipynb).  
3. Once you have run the above mentioned code, you will get out put .py files which we will need in running the ML models. Run them [here](https://github.com/mjaju/Electric_Motor_Temperature/blob/main/Code%20and%20Data%20Files/Machine%20Learning%20Code.ipynb).  
4. Finally run the Complex LSTM model and compare the results ([LSTM code](https://github.com/mjaju/Electric_Motor_Temperature/blob/main/Code%20and%20Data%20Files/Electric_Motor_Temperature.ipynb))  
5. The comparison of the ML and deep learning model has been summarized in this [report](https://github.com/mjaju/Electric_Motor_Temperature/blob/main/Big%20data%20Final%20Report.pdf).  
   
     
The permanent-magnet synchronous machine (PMSM) is an intricate sensor utilized in motion control applications and monitored via infrared sensor guns. The Paderborn University in Germany has been studying temperature regulation of these sensors in an effort to reduce sensor malfunctions. The dataset was acquired from Kaggle.com with the previously expressed goal of temperature prediction derived from eleven PMSM variables. Both machine learning and deep learning techniques were applied to this problem-set. The machine learning techniques included linear regression and random forest regression.  

The linear regression returned a mean square error (MSE) of 0.1971 and adjusted R 2 (adj R 2 ) of 0.8000 on the test set, both results provided a promising baseline for future models. Random forest regression provided the best results of all the models with a MSE of 0.0002 and adj R 2 of 0.9998
with a runtime of less than 20 minutes, making it the team’s proposed candidate to monitor the temperature of the PMSMs. Support vector regression machine learning was determined to be theleast valuable model due to it’s computing time requirements.  
The long short-term memory deep learning models had differing epoch sizes ( epoch = 5, 2, 5) and batch sizes ( batch_size = 1024, 2000, 512). These LSTM models were never able to realize a MSE less than 0.0370 or accuracy greater than 0.9600 while also requiring high computing power for long periods of time, with the quickest epoch taking 1.78 hours to complete. Of the models tested, the random forest machine learning model provided the best results in the second fastest amount of time.  

This accuracy and speed makes it the most practical for field applications and should be deeply considered as the right choice for temperature determination of the PMSM sensors.  
  
  
