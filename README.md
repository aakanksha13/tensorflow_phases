# tensorflow_phases

## Phase I
* Display sample images in the notebook with their corresponding labels
* Split the data into training/validation/test 60:20:20
* Convert to TFRecords format for all the splits
* Build a simple logistic regression model using TensorFlow 2.0
* Train using the training split
* Display the loss and accuracy on Tensorboard
* Validate and display the  validation and test loss
* Add some regularizers (L1, L2, etc.) (Optional)
* Test using the test set
* Compute the accuracy
* Save the model (checkpoint) to disk
* Load the model and make an inference on an image

## Phase II
* Change the logistic to fully connected(FC) neural network (2-layered)
* Change the FC to CNN (inception_v3)

### Phase IV
* Train the inception v3 model with tfrecords that you saved
* Display the summary in tensorboard
* Add early-stopping callback for the training
* Add more metrics (accuracy, precision, recall, etc.)
* Play with parameters to increase the perfomance
   * Fine_at, optimizer, learning rate(exponential decay), etc.
* Add confusion matrix to summary as both image and text

### Phase V
* For multiple image files, save model predictions to a file (Filename,truth,predicted,probabability)
* Add evaluate function that takes a model and tfrecord paths. It returns the accuracy, precision & recall.
* Add image augmentations as a preprocessing of training images:
   - Random horizonal flipping
   - Random cropping
   - Random salt and pepper
   - Random brightness
* Add some random images at the end of each epoch with its true and predicted labels.

\
