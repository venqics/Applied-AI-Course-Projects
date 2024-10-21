**Real world case studies from AppliedAI course**

**1.Human Activity Recognition:**

In this project, I used the data provided by the gyroscope and accelerometer of the smartphone to classify activity that a smartphone user is performing. We have to predict six class labels namely if the user is standing, sitting, laying, walking, walking-upstairs and walking-downstairs. I solved the problem by first building multiple machine learning models(GBDT, random forest, linear SVM, logistic regression, decision trees, RBF SVM)  using domain expert engineered features where linear SVM did a pretty good job giving an accuracy of 96%. While the other approach was using deep learning LSTM cells without domain expert features. It was surprising that a simple two-layered LSTM model was able to achieve an accuracy of 87.5% which is amazing.

**2.Personalized Cancer Diagnosis:**

Applying various machine learning classification techniques on a dataset which contains around 3.3K datapoints of Gene ( Gene causing cancer ), Variations ( Variations in the architecture of amino acids or variations in protein-protein interactions ) and TEXT ( Medical Literature which will help in classifying the type of cancer) . Here our task is to classify the given datapoint consisting information of Gene and Variation into one of the 9 cancer classes mentioned in the dataset using medical literature. The best result was given by Logistic regression by balancing the class points(oversampling) with log loss error of 0.994 versus other models such as linear-SVM, Random forest, Navie Bayes. The models have been both predicted on one-hot encoded features and response-coded features.

**3.Microsoft Malware Detection:**

A Machine Learning approach for classifying a file as Malicious or Legitimate.
This approach tries out 6 different classification algorithms before deciding which one to use for prediction by comparing their results. Different Machine Learning models tried are, Linear Regression, RandomForest, DecisionTree, XGboost, Gradient Boosting, KNN.
In order to test the model on an unseen file, it's required to extract the characteristics of the given file. Python's pefile.PE library is used to construct and build the feature vector and a ML model is used to predict the class for the given file based on the already trained model.

**4.Stack-Overflow Tag Predictor:**

A question in Stack Overflow contains three segments Title, Description and Tags. By using the text in the title and description we should suggest the tags related to the subject of the question automatically. These tags are extremely important for the proper working of Stack Overflow. As the dataset was huge consisting of more than 4 million points which was computationally to hard to train, I tried to train and predict on only a subset of points where logistic regression with one vs rest classifier gave the best results. Also more weightage was given to title feature and feature engineering was don using NLP methods such as stop word removal and TFIDF.

**5.Quora Question Pair Similarity:**

Where else but Quora can a physicist help a chef with a math problem and get cooking tips in return? Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.
Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.
Currently, Quora uses a Random Forest model to identify duplicate questions. In this competition, Kagglers are challenged to tackle this natural language processing problem by applying advanced techniques to classify whether question pairs are duplicates or not. Doing so will make it easier to find high quality answers to questions resulting in an improved experience for Quora writers, seekers, and readers.

