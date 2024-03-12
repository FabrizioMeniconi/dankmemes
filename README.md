# Dankmemes

DANKMEMES task1 Meme Recognition is the development of a project for the EVALITA2020 competition, the details of which are outlined on the following webpage: https://dankmemes2020.fileli.unipi.it/. The task involves training a model for the classification of images and data for the recognition of political memes.


# Description

The project was entirely developed using the Python language in the Google Colab editor, leveraging the Keras and TensorFlow libraries. 
Three network topologies were constructed: the first examines only the images, the second only the additional data related to the images, such as text, manipulation, visual, and engagement. 
Finally, the last one examines all elements of the dataset. To estimate their validity, each model underwent Cross Validation. During training, the training set is divided into 5 subsets, with four used to train the model and the last one to verify the results by calculating accuracy and the value of the loss function. The operation is repeated until all subsets have served as the test set.

Once the 5 training phases are completed, the average and variance of accuracy and the average of the loss for all training sessions are calculated. The best model maximizes accuracy and minimizes the loss function.

# Results

Based on the results of Cross Validation, the best model for each type is chosen. Each of these is retrained using the entire training set, and then evaluated using the test set provided by Evalita. The parameters for performance evaluation include accuracy, precision, recall, and f-measure.

# Installation

It is not possible to provide the dataset as it is owned by Evalita. However, you can open the .ipynb file using the Google Colab editor to see the output of each code segment and the obtained results.
