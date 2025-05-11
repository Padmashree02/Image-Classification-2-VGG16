# Problem - Image classification with Deep neural network

Transfer learning and Fine-tuning a pretrained model is the method to train the model as per the desired output.

> Example- if the model has to classify the new class or optimize the model with more accuracy values.

There are techniques involved in fine-tuning the model, such as either the pre-existing layers can be freezed and change the last layer, or tweak the already trained layers as per our need.

> My solution of fine-tuning is by adding my custom output layers with the trained layers (pre-existing layers) of the model and while training, the model will be trained with addition of new layers.

Solution :-

  > Network/Layer - VGG16

  > Framework - Tensorflow (Tensorflow.Keras)

  > Dataset (while training the network) - Tensorflow dataset/"citrus_leaves"

  > Library - cv2, numpy, matplotlib.pyplot

  > Topic - VGG16, layers, optimizers, tfds, image generator, loss, accuracy

  > Pipeline :-
 
      : import the model from tensorflow.

      : Load the required datasets from the tensorflow detasets into train and valid respectively.

      : Preprocess the dataset as per the VGG16's network configuration.

      : Perform image generator to each pre-processed dataset (train and valid).

      : Intialize the VGG16 network with its own weights.

      : Define the custom layers.

      : Configure the model.

      : Train with pre-existing layers, new layers and new dataset.

      : Evaluate the trained model to anlayse how well the model has been trained in training phase.
      
      : Test the trained model with new images, to test how well the model reacts with new images. 

  > Result - The VGG16 with new output layers has yield an accuracy of 85 % .
