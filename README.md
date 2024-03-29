> ## [Read Paper Here](https://www.researchgate.net/publication/366121073_A_Deep_Learning_Multi-Class_Time_Series_Classification_Approach_for_Human_Activity_Recognition?_sg%5B0%5D=Fqcd0GJfkI4SbOwUv75bRAhbVJ_L0M17kSW7PJAIR5F2umpPeDX9pF_pr-iD2mKLfdRAOsO32YeW7_CzdQfm95vtSz9DyVVVulQDSlGY.9lY7lCZmglY_ZEqRIN3Ricq6aEterBoxFJDE_mgunu9SpssFWVOGPGBwGRUuk4BxBTGiaihG4VmNOFWMbacKww)

# A Deep Learning Multi-Class Time Series Approach for Human Activity Recognition

![image](https://github.com/syedhadi816/human-activity-recognition-with-deep-learning-multi-class-time-series-classification/assets/53166976/fd8981f5-9be5-4886-a4c4-fc64f0e0b48d)
Image Source: HAR (Human Activity Recognition Using Smartphones), Davide Anguita et al. in A Public Domain Dataset for Human Activity Recognition using Smartphones

### Description

Activity recognition is the problem of predicting movement and detecting activity of a person from sensor data. These sensors are often accelerometers and gyroscopes, and they capture activity data when mounted as smartphones or wearables (smart watches). It has been an active area of research recently since wearables (particularly for fitness tracking) are gaining popularity. Activity recognition data is collected over time as a subject performs an activity and the sensor tracks movements over fixed intervals of time. However, the problem of activity recognition is approached either as single point classification or as time series classification. The advantage in using time series classification is that it allows to model upon the temporal coherence information that is made available as an activity is recorded over a time interval rather than as a single point observation. 

For this project, we will be using a rather simplistic dataset that contains accelerometer data from 15 subjects who perform a variety of tasks. Data is collected as acceleration in 3 dimensions (x, y and z axes). We will be expanding on the existing research on this dataset by applying deep learning multi class time series classification algorithms to identify the activity. Previously, the dataset has been used with single point ensemble classification algorithms. We will be exploring the advantage of taking into account the temporal information of this dataset. Existing single point classification algorithms will also be implemented to benchmark the results. 

Previously the approach of time series classification has been successful on a more complex dataset (UCI HAR dataset) with accelerometer and gyroscope sensors, the dataset is more complex in terms of the sensor information (having 560 features on localization information of subjects). The goal of this project is to understand whether the added complexity of a multi-layer deep learning time series classification algorithm offers significant benefits in terms of the efficiency and the predictability when only accelerometer data is available (having only 3 features on acceleration information of subjects). 


### Proposed Methodology

For the purpose of activity recognition using the accelerometer data of subjects, we will primarily be testing multi-class time series classification algorithms. We will be testing out convolutional neural networks (specifically 1D CNNs) and recurrent neural networks (specifically LSTMs). Additionally, Bi Directional LSTM will also be tested. The results of these models will be compared to single point classification approaches (KNN and ensemble random forests). For the purpose of this experiment, these fixed-point classifiers will also be created to validate on the results on the same data that is prepared for the time series classification models. 

### Evaluation Metrics

To evaluate the models that will be built, we will be using confusion matrices, ROC curves and AUC curves. Estimates of the overall accuracy, recall, F-1 and precision will be compared across the models. The primary goal is to compare the best single point classifier with the best time series classifier using the evaluation metric metrics identified. 


