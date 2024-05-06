# SMS-SPAM-Classification

Project Objective : The objective of this project is to develop a machine learning model that can accurately classify SMS messages as spam or non-spam.The ultimate goal is to create a reliable and efficient system for detecting and filtering out spam messages, thereby improving user experience and security in SMS communication.

Data Sources: Data was collected from the Kaggle.It is containing informatio about the SMS Spam Collection, is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.Link(https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

Libraries : Pandas, Numpy, SK-learn, Streamlit, NLTK(Word_tokenization, Stopwords_removal, Stemming, Text_vectorization)

EDA Observations:
>>There is class imbalancing in target column(Ham : 87.3% , Spam : 12.63%) after dropping duplicate values.
>>Hum class contains more no of words and Spam class contains less no words.
>>We created 3 new cloumns from text cloumns : num_sent, num_words, num_characters.

Text Preprocessing: Here, we converted the 'text' column to 'transformed_text', applying word tokenization, stopwords removal, and stemming to clean the data after that we applied text vectorization. And also generated the word_cloud with respect to 'ham' & 'spam' class.

Model Building: We have created multiple models-

Model Name -  Multinomial NB |
Accuracy -  0.9709864603481625 |
Precision -  1.0 |
_______________	
Model Name -  SVC |
Accuracy -  0.9758220502901354 |
Precision -  0.9747899159663865 |
_______________
Model Name -  KN |
Accuracy -  0.9052224371373307 |
Precision -  1.0 |
_______________
Model Name -  DT |
Accuracy -  0.9323017408123792 |
Precision -  0.8333333333333334 |
_______________
Model Name -  LR |
Accuracy -  0.9584139264990329 |
Precision -  0.9702970297029703 |
_______________
Model Name -  RF |
Accuracy -  0.9758220502901354 |
Precision -  0.9829059829059829 |
_______________
Model Name -  AdaBoost |
Accuracy -  0.960348162475822 |
Precision -  0.9292035398230089 |
_______________
Model Name -  GBDT |
Accuracy -  0.9468085106382979 |
Precision -  0.9191919191919192 |
_______________
Model Name -  xgb |
Accuracy -  0.9671179883945842 |
Precision -  0.9262295081967213 |

Model Selection : As we can see there are 2 models which are performing very well in terms of precision KNN_classifier(1) and Multinomial naive bayes(1) but when it comes to accuracy we will go ahead with MultinomialNB model.
