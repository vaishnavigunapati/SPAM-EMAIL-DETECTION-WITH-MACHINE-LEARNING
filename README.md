# SPAM-EMAIL-DETECTION-WITH-MACHINE-LEARNING
#CODECASA/
             TOPICS
-INTRODUCTION
-PROBLEM STATEMENT
-OBJECTIVE
-METHODOLOGY
-CONCLUSION

ABSTRACT-
The upsurge in the volume of unwanted emails called spam has created an intense need for the development of more dependable and robust antispam filters. Machine learning methods of recent are being used to successfully detect and filter spam emails. We present a systematic review of some of the popular machine learning based email spam filtering approaches. Our review covers survey of the important concepts, attempts, efficiency, and the research trend in spam filtering. The preliminary discussion in the study background examines the applications of machine learning techniques to the email spam filtering process of the leading internet service providers (ISPs) like Gmail, Yahoo and Outlook emails spam filters. Discussion on general email spam filtering process, and the various efforts by different researchers in combating spam through the use machine learning techniques was done. Our review compares the strengths and drawbacks of existing machine learning approaches and the open research problems in spam filtering. I recommended deep leaning and deep adversarial learning as the future techniques that can effectively handle the menace of spam emails.

INTRODUCTION-
Emails are important because they creates a fast, reliable form of communication that is free and easily accessible. They allow people to foster long-lasting, long-distance communication . Spam e-mails can be not only annoying but also dangerous to customers.Spam e-mails can be defined as

*Anonymity
*Mass-Mailing
*Unsolicited Spam e-mail messages are randomly sent to multiple addresses by all sort of groups , but mainly by lazy advertisers and criminals who wish to lead you to phishing sites.

PROBLEM STATEMENT-
I have chosen this project because nowadays there are lots of people trying to fool you just by sending you fake e-mails like you have won a 1000 dollars, this much amount is deposited in your account once you open this link and then they will try to hack your information.

Unwanted emails irritating internet consumers.
*Critical e-mail messages are missed and/or delayed.
*Identity Theft.
*Spam can crash mail servers and fill up hard drive.
*Billions of dollars lost worldwide.

OBJECTIVE-
The objective of identification of spam e-mails are :

*To give knowledge to the user about the fake e-mails and relevant e-mails.
*To classify that mail is spam or not.

METHODOLOGY-
METHODOLOGY	                   DESCRIPTION
Collecting Dataset	The test data is used to check the accuracy of the model built with the training data. The training data set contains 4137 emails . The test data 
                     contains 1035 emails
Data Preprocessing	For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a proper manner. STOP WORDS 
                    ,CREATING WORD DICTIONARY
Feature Selection 	Once the dictionary is ready, I can extract word count vector (our feature here) of 3000 dimensions for each email of training set. Each word count vector              contains the frequency of 3000 words in the training file.
Model Construction	Naive Bayes ,logistic Regression , SVM

STEP BY STEP PROCESS
DATA PREPROCESSING-
The emails in the learning data are in plain text format. I need to convert the plain text into features that can represent the emails. Using these features we can then use a learning algorithm on the emails. A number of pre-processing steps are first performed like normalization , binary data.. convert the plain text files to files with one word per line. In this project, I look at emails just as a collection of words. So, to make it easier I convert each file into a list of words.

Why is Data Preprocessing important?-
For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a proper manner. Some specified Machine Learning model needs information in a specified format, for example, Random Forest algorithm does not support null values, therefore to execute random forest algorithm null values have to be managed from the original raw dataset.

STOP WORDS-
There are some English words which appear very frequently in all documents and so have no worth in representing the documents. These are called STOP WORDS and there is no harm in deleting them. Example: the, a, for etc. There are also some domain specific (in this case email) stop words such as mon, tue, email, sender, from etc. So, delete these words from all the files.

FEATURE EXTRACTION PROCESS-
Once the dictionary is ready, we can extract word count vector (our feature here) of 3000 dimensions for each email of training set. Each word count vector contains the frequency of 3000 words in the training file. Of course you might have guessed by now that most of them will be zero. Let us take an example. Suppose we have 500 words in our dictionary.
Each word count vector contains the frequency of 500 dictionary words in the training file. Suppose text in training file was “Get the work done, work done” then it will be encoded as [0,0,0,0,0,…….0,0,2,0,0,0,……,0,0,1,0,0,…0,0,1,0,0,……2,0,0,0,0,0]. Here, all the word counts are placed at 296th, 359th, 415th, 495th index of 500 length word count vector and the rest are zero.


NAIVE BAYES CLASSIFIER-
A Naive Bayes classifier is a probabilistic machine learning model that’s used for classification task. The crux of the classifier is based on the Bayes theorem.Bayes Theorem: For example, a fruit may be considered to be an apple if it is red, round, and about 3 inches in diameter. Even if these features depend on each other or upon the existence of the other features, all of these properties independently contribute to the probability that this fruit is an apple and that is why it is known as ‘Naive’.

P(A/B) = P(B/A)P(A)/P(B)


LOGISTIC REGRESSION-
Logistic regression is a supervised machine learning algorithm mainly used for classification tasks where the goal is to predict the probability that an instance of belonging to a given class. It is used for classification algorithms its name is logistic regression. it’s referred to as regression because it takes the output of the linear regression function as input and uses a sigmoid function to estimate the probability for the given class. The difference between linear regression and logistic regression is that linear regression output is the continuous value that can be anything while logistic regression predicts the probability that an instance belongs to a given class or not.
Logistic Regression Equation
The odd is the ratio of something occurring to something not occurring. it is different from probability as the probability is the ratio of something occurring to everything that could possibly occur. so odd will be

\frac{p(x)}{1-p(x)}  = e^z  

Applying natural log on odd. then log odd will be

\log \left[\frac{p(x)}{1-p(x)} \right] = z \\ \log \left[\frac{p(x)}{1-p(x)} \right] = w\cdot X +b  

then the final logistic regression equation will be:

p(X;b,w) = \frac{e^{w\cdot X +b}}{1+e^{w\cdot X +b}} = \frac{1}{1+e^{-w\cdot X +b}}  


SUPPORT VECTOR MACHINE-
Support vector machines (SVMs) are powerful yet flexible supervised machine learning algorithms which are used both for classification and regression. But generally, they are used in classification problems.
An SVM model is basically a representation of different classes in a hyperplane in multidimensional space. The hyperplane will be generated in an iterative manner by SVM so that the error can be minimized. The goal of SVM is to divide the datasets into classes to find a maximum marginal hyperplane (MMH).
SVM kernel converts non-separable problems into separable problems by adding more dimensions to it. It makes SVM more powerful, flexible and accurate.(Linear,gaussian,polynomial,rbf).

CONCLUSION-
I was able to classify the e-mails are spam or non-spam .With high number of e-mails lots if people using the system it will difficult to handle all possible mails as our project deals with only limited amount of corpus.
I can now take raw input from the user and classify it as spam or ham.
