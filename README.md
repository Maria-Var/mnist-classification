# MNIST Classification model (for recognition of handwritten digits 0..9).


**Python packages used for data preprocessing and creating of the model:** TensorFlow

**Input:** dataset of images of handwritten digits, labeled as 0..9. 60000 training and 10000 test images.

**Data preprocessing:**
- **Flatten**: Every image has size of 28px * 28px. That is 784 features for each image.
- **Standardize**: as every feature has value of [0, 255] (the intensity of grey, from black to white), we standardize it by dividing every element on 255.

**Model:**
Neural Network (6 layers):
- Optimization algorithm: Adam
- Activation functions: layers 1, 2, 3, 4, 5 – ReLU, and layer 6 – softmax

Hyperparameters of the Neural Network:
-	Depth: 5 hidden layers
-	Width: size of hidden layers = 400, size of output layer = 10
-	Mini-batch size: 100
-	Learning rate: 0.0075
-	Number of epochs: 6	

**Result:** prediction accuracy – 97.29% on the test dataset.