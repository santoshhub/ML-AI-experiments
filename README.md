# Sentiment Analysis
====================
 * Sentiment Analysis is performed on Amazon Jewelry Dataset link, https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Jewelry_v1_00.tsv.gz
 * Dataset details - https://huggingface.co/datasets/amazon_us_reviews
 * Feature Extraction, TF-IDF: It is a method of extracting the features from the text data. TF stands for Term Frequency and IDF stands for Inverse Document Frequency
 * Models used: SVM classifier & Logistic Regression
 * SVM classifier, accuracy of 91.55%
 * LR classifier, accuracy of 91.80%
 
# MNIST Dataset Prediction Using Keras
====================
* MNIST is "Modified National Institute of Standards and Technology." This dataset consists of handwritten digits from 0 to 9, and it provides a platform for testing image processing systems.
* MNIST prediction is using the dataset: https://storage.googleapis.com/tensorflow/tf-keras-datasets/mnist.npzIn preprocessing, the original image of 28 pixels by 28 pixels is normalized to 255 RGB.
* Model training uses the Keras library to stack the image into a dense pool of layers, stacking each layer on top of the others. It uses relu’ as activation function, and stacked a few more layers with ‘softmax’ as our activation function. Then, finally, we compile the entire model which uses mean_squared_error as our loss function. To optimize our model, use Adam.  Used epochs = 10 and batch_size = 100. 
* Model evaluation: the model has 98.30% accuracy. 
* Model serving: the model is saved in protobuf format on the drive. Used the tensorflow_model_server to serve the request over REST. 
