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

   Algorithm	  Accuracy	Precision
1	KN	  0.905222	1.000000
4	RF	  0.975822	0.982906
0	SVC	  0.975822	0.974790
3	LR	  0.958414	0.970297
5	AdaBoost  0.960348	0.929204
7	xgb	  0.967118	0.926230
6	GBDT	  0.946809	0.919192
2	DT	  0.932302	0.833333
