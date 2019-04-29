# MusicMoodPrediction
 
1. Dataset Preparation
2. Feature Engineering
3. Create NLTK Models on the Dataset
4. Create Machine Learning Models
5. Measure Accuracy and Confusion Matrix on English Songs
6. Create Test Dataset for Hindi Songs
7. Translate to Hindi
8. Test Dataset Pre-processing
9. Accuracy score for Hindi Bollywood Movie Songs

## Predict mood of the song from lyrics
Digitization of music has led to easier access to different forms music across the globe. Increasing work pressure denies the necessary time to listen and evaluate music for a creation of a personal music library. One solution might be developing a music search engine or recommendation system based on different moods. Develop a mood classification system from lyrics as well by combining a wide range of semantic and stylistic features extracted from textual lyrics.

## Dataset and the code used
Here we took the training data of four moods namely, happy,sad, angry, relaxed and the test data for hindi songs has been generated for testing. Dataset used can be found at https://drive.google.com/file/d/1GFBIJwFYzcpsu3lkCdauGW_0mKpk-uSj/view?usp=sharing.
Here we do data preprocessing inside Mood_Prediction.ipynb and feed to feature engineering models like count vectorizer model,TfodfVectorizer Model, Tfidf-NGram Model. Now the modified dataset is used in prediction models like Random Forest, Logistion regression, SVM, and multinomial naive baise, to preict the test data set and plot the confusion matrix.At the end there is a function that takes in a random hindi song in romanized format, translates it to english lyrics using google trans and then preprocess it to feed it to particular model and predict its mood.

## Project Workflow
Download Million Song subset from https://labrosa.ee.columbia.edu/millionsong/ and download NJU dataset from https://cs.nju.edu.cn/sufeng/data/musicmood.htm . Now run Data_Preparation.ipynb to create training dataset "training_backup.csv" and testing dataset "testing_backup.csv". Now run Mood_Prediction.ipynb to create machine learning models for mood prediction using lyrics. At last, pred() and pred1(), two functions are given, which takes song lyrics, in English and Hindi respectively to predict the mood of the song.

