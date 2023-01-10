# MUZik
It is a Recommendation System that recommends songs to users according to their mood/emotion.
The resources required for developing this project include:
  1. Anaconda (Jupyter Notebook)
  2. Pycharm (for integrating the modules developed)
  3. Spotify Developer account
The whole project is divided into 4 modules:
Module 1: Facial Expression Detection
Module 2: Music Recommendation System
Module 3: User Interface (UI)
Module 4: Integrating module 1 and module 2 with UI

MODULE-1: Facial Expression Detection

As the project is recommending songs on mood, the mood of the user can be identified through webcam of their device from the facial expressions.
Technologies used in this module:
  -CNN Algorithm(Convolutional Neural Networks)
  -OpenCV
 CNN algorithm is used in identifying the facial expressions of the user.
 Here, for training the model, we have taken the dataset from kaggle.
 With the help of this data, we have trained and tested the facial expression detection model using CNN algorithm and got an accuracy of 64.5 %.
 This model that is trained is saved in the file "model.h5".
 As the system resources aren't supporting such huge data, we trained our CNN model on kaggle itself.
 
 MODULE-2: Music Recommendation System
 
 In this module, we used a dataset of approx. 167,000 rows with each row being a sing with different features like acousticness, dancebaility, etc.
 Based on these features, we've trained our model using "catboost algorithm" as it gave the best accuracy among all the other classification algorithms we've used.
                                                              ALGORITHM                ACCURACY
                                                              KNN	                       74.3
                                                              NAÏVE BAYES 	             78.8
                                                              SVM	                       79.7
                                                              RANDOM FOREST	             79.7
                                                              LOGISTIC REGRESSION	       80.6
                                                              XGBOOST	                   81.9
                                                              LGBM	                     83.7
                                                              CATBOOST	                 94.2
This model can help in classifying the mood of any new song with all the mentioned features.

MODULE-3: User Interface

User Interface was developed initially by taking some images and merging them together to form static backgrounds in Canva.
Later, the canvas dimensions were set in 3D Paint.

MODULE-4: Integration of Module 1 and Module 2

Here, we have linked the first 2 modules in pycharm to create the flow.
We have used Tkinter for developing this as it is supported for Python codes.


