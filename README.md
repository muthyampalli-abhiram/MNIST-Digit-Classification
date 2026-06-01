So I wanted to check the perfomace of a Single Layer Perceptron, a Multi Layer Perceptron and the CNN on the MNIST Dataset.
Step-1:
Loaded the dataset
Step-2:
Separated features and target labels]
Step-3:
splitted the data into train test x_train,x_test,y_train,y_test
Step-4:
Normalized the values of x_train and x_test by dividing them with 255.0
Step-5:
converted x_train,x_test from dataframes to Numpy Array.
Step-6:
Reshaped x_train and x_test to (28,28,1) as cnn requires input in (height,width,channels) format.
Step-7:
Since I made use of categorical_crossentropy as loss function so I need to encode my target labels.
Therefore, the target labels were encoded using to_categorical
step-8:
Build a Single Layer Perceptron compiled and fitted it to the data.
Step-9:
Build a Multi Layer Percpetron compiled and fitted it to the data.
Step-10:
Finally, built a CNN model with 2 convolutional layer along with 2 MaxPool layers compiled it and fitted with the data.

At Last, the training accuracy and the validation accuracy curve fo CNN was a achieved to be a perfect curve than Single Layer Perceptron and Multi Layer Perceptron.
I cam to know that CNN performs well on Images than a single Layer Perceptron and a Multi Layer Perceptron.

Dataset Link : https://www.kaggle.com/datasets/animatronbot/mnist-digit-recognizer
Tensorflow : https://www.tensorflow.org/
