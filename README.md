# foodback-machine-learning

# Modelling Foodback

This model use to classify image based on the input. By using the model, will predict which class the food in the image belongs to among the 69 classes modeled.

# foodback_modelling.ipynb

## Foodback Food Image Classification Model
## A. How to Make the Model?

i. Data Pre-processing
1. Load the dataset from local using `os` library. 
2. Check the class name to be modeled
3. Image Augmentation

ii. Modelling Process
1. Define the model. In this scoop, the model uses:
  - 2 layers of Keras Dropout layer, and
  - 3 layers of Keras Dense layer. 

The activation function used in the model is `ReLu` for the first two layers of Keras Dense layer and the activation function for the third Keras Dense layer is `softmax` used to do multi-class classification.
2. Define the model input and output. 
3. Compile the model. The loss function used in this model is the `categorical_crossentropy`. To fit this model better, `Adam` is used for optimization and `accuracy` as the metric.  
4. Fit the model with epoch of 100.
 

iii. Evaluation
Evaluation process aims to evaluate how the model works, and how the model converges through each epoch. There are two graphs to be made, the accuracy plot, and the loss plot.

1.  Accuracy Plotting
Plot the accuracy of both the train set and the test set in the epoch. Evaluate model from accuracy  fluctuations and movement to decide if the model is well-fit or not.

2. Loss Plotting
Plot the loss of both the train set and the test set in the epoch. Evaluate model from loss fluctuations and movement to decide if the model is well-fit or not.

3. Table of model accuracy and loss

   | Accuracy | Val_accuracy | Loss   | Val_loss | Model    |
   | -------- | ------------ | ------ | -------- | -------- |
   | 0.8164   | 0.7881       | 0.6217 | 0.7400   | Good fit |
